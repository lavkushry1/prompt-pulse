# Prompt Pulse: The "No Bullsh*t" Guide to Code That Doesn't Suck (Solo Ops Edition)

**Purpose:** This is our contract. These are the rules for building Prompt Pulse. Follow them. If your AI brain gets clever ideas about "optimizing" for obscurity, reboot that thought. Simple, maintainable, and *it works*. That's the goal. Our time is the only resource we can't buy more of as a solo dev.

**Note for AI Tools (aka Cursor, My Digital Minion):** You are here to make me faster, not to create puzzles. Before you generate a single line of code for Prompt Pulse, you *will* internalize these rules. Your output will be judged harshly. Reference other docs for context, but these principles are your core directive.

---

## 👑 Why Code Quality is King (Founder's Non-Negotiable Decree)

As a solo dev, my sanity and the success of this SaaS depend on this:

1.  **Ship Fast, Fix Faster:** Clean code means I can actually find and fix bugs, or add new niche features, without a week of archaeology. Less mess = more value, faster.
2.  **My Future Self Thanks Me:** The code I write (or you generate) today, I have to live with. Make it understandable.
3.  **Bugs are Time Thieves:** Every stupid bug from lazy code steals time I could be using to talk to users or build what they actually pay for. Fewer bugs = more money.
4.  **Complexity is the Enemy:** This thing needs to scale when it gets users, not when the code itself becomes a monster. Keep it simple so I can optimize *when* and *where* it matters.
5.  **Focus:** I can't afford to burn out untangling your AI's idea of "elegance." Clear code lets me focus on the product.

**Bottom Line: Quality isn't a 'nice-to-have.' It's the foundation of not failing.**

---

## 🛠️ The Only Coding Principles That Matter (for us):

Three rules. Learn them. Live them.

### 1. DRY (Don't Repeat Yourself) – Stop Wasting My Time & Bytes.

*   **The Deal:** If you find yourself writing the same (or damn similar) chunk of logic or UI more than twice, **STOP**. That's a function. That's a component. That's a utility.
*   **Why I Care:** Bugs fixed once. Features changed once. Less code for me to scroll through.
*   **Examples for Prompt Pulse:**
    *   API call wrappers (for LLMs, for integrations).
    *   Common UI elements (our buttons, modals, inputs better look and act the same).
    *   User role checks.
    *   Analytics logging.
*   **Your Job (AI):** Before generating, sniff around for existing code that does the job. Use it. If something *should* be reusable but isn't, flag it for me to refactor or suggest how to make it a reusable module.

### 2. KISS (Keep It Simple, Stupid) – Your "Smart" Is My "Problem."

*   **The Deal:** Write the most straightforward code that *actually works* and solves the problem. No fancy algorithms for simple tasks. No ten-layer abstractions when one function will do.
*   **Why I Care:** I can read it. I can debug it. It probably has fewer hidden bugs.
*   **Examples for Prompt Pulse:**
    *   Integration: Call the specific API endpoints we need. Don't build a generic client for the entire damn service unless I tell you to.
    *   State: Use React's built-in state. If it gets *really* messy (and I'll be the judge), *then* we talk global state managers.
    *   DB: Simple, readable queries.
    *   Components: Do one thing. Do it well.
*   **Your Job (AI):** Generate the most direct solution first. If you think something needs to be complex, justify *why* the simple way won't cut it *for the current task*. Add comments only if the code isn't blindingly obvious (and if it's not, question why).

### 3. Modularity – Small Pieces, Loosely Joined. That's It.

*   **The Deal:** Break things down. Functions are small. Components are small. Modules handle one area of concern. They talk through well-defined doors (APIs, props), they don't barge into each other's rooms.
*   **Why I Care:** I can test bits in isolation. I can change one part without breaking ten others. I can actually find things. I can reuse things (see DRY).
*   **Examples for Prompt Pulse:**
    *   Backend: Auth service. LLM service. Separate services for each bloody Integration. Webhook handlers.
    *   Frontend: A `Button` component. An `Input` component. A `Modal` component. Specific UI sections are their own components. Utilities for date formatting, validation, etc., are in their own files.
    *   Extension: Background, content, popup are separate worlds with clear message passing.
*   **Your Job (AI):** Think small. Generate focused pieces of code. Put them in the right damn directory. If you're creating a file that's 500 lines long for a simple feature, you've failed.

---

## 🤖 My Rules for You, AI Coding Minion (Cursor & Friends):

You're fast. That's your only advantage. Don't squander it by making my life harder.

1.  **Context First, Code Later:** Before you spit out code, *read* the User Story, the Tech Stack doc, the Task Breakdown, the UI/UX Guide, and *this* doc. Know *what* you're building and *why*, and *how I expect it built*.
    *   **Example Me -> AI:** "Bot, User Story #5: Integrated Contextual Suggestions. Review `UI/UX Guide Section 3` and `Tech Stack: Chrome Extension Layer`. *Then* generate the content script for Hubspot detection."
2.  **KISS is Your God:** Simplest code that works. No showing off. If a simple `if` statement works, don't give me a strategy pattern.
    *   **Example Me -> AI:** "Implement the feature gating. Simplest approach that checks user role and works."
3.  **DRY or Die Trying:** Scan for reusable code *before* you write new stuff. If you generate something that duplicates existing logic, I'll know.
    *   **Example Me -> AI:** "Implement save output. We already have an API call utility and a modal component. Use them."
4.  **Modules, Not Monoliths:** Small, focused functions/components. Correct file paths. Don't make me refactor your mess into sensible modules.
    *   **Example Me -> AI:** "Write the `IntegrationConnectButton` React component. It handles OAuth initiation. Put it in `components/integrations/`."
5.  **TypeScript & My Conventions. Period.** My project, my rules. ESLint and Prettier are not suggestions. Functional React components. Async/await.
    *   **Example Me -> AI:** "Generate TypeScript code for this API endpoint. Make sure it passes ESLint and Prettier checks for this project."
6.  **Explain Yourself (Briefly):** If the code isn't obvious (and if it's not, see KISS), add a comment explaining *why* it's like that. For major chunks you generate, give me a one-liner on its purpose.
    *   **Example Me -> AI:** "Generate the OAuth callback handler. Add a comment explaining the token exchange and secure storage step."
7.  **Security Isn't Optional:** If it touches user data, auth, or external systems, your first thought is "how can this be exploited?" Build defensively. Validate inputs on the server. Don't leak secrets. If you're unsure about a security aspect, *flag it explicitly*.
    *   **Example Me -> AI:** "Implement backend for user profile update. Ensure all inputs are validated server-side using Zod schema `UserProfileSchema` and user is authorized to update *their own* profile only."
8.  **One Task, One Commit (Figuratively):** Focus on the specific task from the "Dev Task Backbone." Don't try to build the whole damn product in one go. Small, verifiable steps.
    *   **Example Me -> AI:** "Implement ONLY Step 4.2: 'Implement Free Tier Usage Limits (Add Usage Counter)'."
9.  **If You're Confused, Ask. Don't Assume.** Ambiguity means bugs. If a requirement is fuzzy, or you see two vastly different ways to do it, ask me for clarification. Don't just pick the most complicated one.
    *   **Example Me -> AI:** "For the integration API call, the docs mention two authentication methods. Which one aligns with our project's security standards (`000-project-standards.mdc`)?"
