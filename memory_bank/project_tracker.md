# Prompt Pulse: Level Up Log (Progress Tracker) 🎮🔥

**Purpose:** This is our live feed on where Prompt Pulse is at. Tracks every W from the "Dev Task Backbone." When a task is crushed, we update it here. Simple.

**Note for AI Tools (Yo, Cursor!):** This is your main HUD. You finish a sub-task? Change that `[ ]` to `[x]`. Got an important link or a note on what you did? Drop it in "Output/Note." Keep this fresh, aight?

**Key:**
*   `[ ]`: Task LFG (Let's F***ing Go - Not Started)
*   `[x]`: Task GGs (Good Game - Completed)
*   `[🚧]`: Task WIP (Work In Progress - Stuck or Mid-Grind)

---

## 🚀 Phase 1: Lvl 1 - Laying the Foundation (Niche Strategy & Core Infra)

**Boss Goal:** Confirm our niche is legit & the base build is solid.
**Founder's Vibe:** No cap, if this phase fails, we pivot hard or bail. This is foundational.

### Mission: Define Niche & Problem Scope

*   `[ ]` **1.1.1:** Vibe Check Niche: User Interviews (Target: 20-30 DMs/calls)
    *   *Output/Note (e.g., Pain points, common tools used):*
*   `[ ]` **1.1.2:** Map Niche Flow: Identify daily grind, tools, biggest Ls.
    *   *Output/Note (e.g., Visual workflow map link):*
*   `[ ]` **1.1.3:** Tool Recon: Scope top 3 Niche tools & their API sitch (read/write access).
    *   *Output/Note (e.g., API feasibility report link):*
*   `[ ]` **1.1.4:** Quantify the Bag: Estimate time/money saved for Niche users.
    *   *Output/Note (e.g., ROI projection doc link):*
*   `[ ]` **1.1.5:** Lock In Decisions: Doc Niche, Main Problem, 1st Integration Target.
    *   *Output/Note: Link to Niche Decision Doc:*

### Mission: Project Genesis

*   `[ ]` **1.2.1:** Git Repo Online (GitHub/GitLab)
    *   *Output/Note: Repo URL:*
*   `[ ]` **1.2.2:** CI/CD Pipeline GO (Vercel/Netlify/GCP Cloud Build)
    *   *Output/Note: Main Deployment URL:*
*   `[ ]` **1.2.3:** Bootstrap Next.js/React Stack (TypeScript, Tailwind)
    *   *Output/Note: Initial commit hash:*
*   `[ ]` **1.2.4:** Style Config Locked (`tailwind.config.js` & `globals.css`)
    *   *Output/Note:*
*   `[ ]` **1.2.5:** TypeScript Config Locked (`tsconfig.json`)
    *   *Output/Note:*

### Mission: Auth Layer Setup

*   `[ ]` **1.3.1:** Integrate Auth Service (Clerk/Firebase Auth) - SDK setup done.
    *   *Output/Note: Chosen Auth Service:*
*   `[ ]` **1.3.2:** Build Basic Signup/Login UI.
    *   *Output/Note: Component file paths:*
*   `[ ]` **1.3.3:** Secure Backend Auth Endpoints (e.g., session management).
    *   *Output/Note: Endpoint paths:*
*   `[ ]` **1.3.4:** Define User Roles (free/pro/team) in Auth & DB.
    *   *Output/Note:*

### Mission: Database Base Camp

*   `[ ]` **1.4.1:** DB Provisioned (Supabase/PostgreSQL instance up).
    *   *Output/Note:*
*   `[ ]` **1.4.2:** Schema Drafted & Applied: `users` table (Migration file link).
    *   *Output/Note:*
*   `[ ]` **1.4.3:** Schema Drafted & Applied: `subscriptions` table (Migration file link).
    *   *Output/Note:*
*   `[ ]` **1.4.4:** Schema Drafted & Applied: `niche_outputs` (basic) (Migration file link).
    *   *Output/Note:*
*   `[ ]` **1.4.5:** Schema Drafted & Applied: `integration_credentials` (Migration file link; *Encryption Notes:* ).
    *   *Output/Note: Encryption notes updated.*
*   `[ ]` **1.4.6:** Basic Row Level Security (RLS) Policies Applied.
    *   *Output/Note: RLS policy names/links.*

---

## 🎯 Phase 2: Lvl 2 - First AI Drop (Core Niche Workflow MVP)

**Boss Goal:** Get the first AI-generated output live for our main niche task.
**Founder's Vibe:** Show, don't tell. Get that core AI magic working, fast.

### Mission: Design Niche Workflow Interface

*   `[ ]` **2.1.1:** Implement Input Form UI Component for MVP Niche Task.
    *   *Output/Note: File path:*
*   `[ ]` **2.1.2:** Implement Output Display UI Component.
    *   *Output/Note: File path:*

### Mission: Build LLM Backend

*   `[ ]` **2.2.1:** Create `/api/generateNicheOutput` Endpoint.
    *   *Output/Note: File path:*
*   `[ ]` **2.2.2:** Integrate Basic LLM Call (e.g., GPT-3.5-turbo, test with model chosen in LLM Juice Strategy).
    *   *Output/Note: Confirm model selection for MVP.*
*   `[ ]` **2.2.3:** Define MVP Niche Prompt & Implement Prompt Assembly.
    *   *Output/Note: Link to prompt version/template doc.*
*   `[ ]` **2.2.4:** Implement Basic LLM Response Handling & Error Logging (Sentry connected).
    *   *Output/Note:*

### Mission: Connect Frontend <> Backend

*   `[ ]` **2.3.1:** Wire Input Form to `/api/generateNicheOutput`.
    *   *Output/Note:*
*   `[ ]` **2.3.2:** Wire Backend Output to Frontend Display.
    *   *Output/Note:*

### Mission: Niche Output Formatting

*   `[ ]` **2.4.1:** Implement Logic to Format Raw LLM Output for [Niche Task] (e.g., email structure).
    *   *Output/Note: Example output format committed.*

---

## 🔗 Phase 3: Lvl 3 - First Link-Up (Key Integration MVP)

**Boss Goal:** Get data flowing from our #1 Niche Tool & send output back.
**Founder's Vibe:** This is where we flex. Integration is our MOAT.

### Mission: Recon 1st Integration API ([Integration Name])

*   `[ ]` **3.1.1:** Map MVP API Endpoints: Read Context, Basic Apply/Write.
    *   *Output/Note: API endpoint mapping doc link.*
*   `[ ]` **3.1.2:** Document OAuth Flow.
    *   *Output/Note: OAuth flow diagram/notes link.*
*   `[ ]` **3.1.3:** Document Rate Limits & Error Codes.
    *   *Output/Note:*

### Mission: Build Integration Backend ([Integration Name])

*   `[ ]` **3.2.1:** Implement OAuth & Secure Token Storage [Security Check: Passed].
    *   *Output/Note: Token refresh logic implemented.*
*   `[ ]` **3.2.2:** Backend Module: Fetch Context Data via API.
    *   *Output/Note: File path: `services/integrations/[integration_name].ts`*
*   `[ ]` **3.2.3:** Backend Module: Basic "Apply" Action via API.
    *   *Output/Note: File path: `services/integrations/[integration_name].ts`*
*   `[ ]` **3.2.4:** Error Handling & Retries for API Calls.
    *   *Output/Note: Implemented using [Retry Library/Pattern].*

### Mission: Build Integration Frontend ([Integration Name])

*   `[ ]` **3.3.1:** UI: "Connect to [Integration Name]" Button (OAuth flow start).
    *   *Output/Note: Component file path.*
*   `[ ]` **3.3.2:** UI: Select/Display Context Pulled from [Integration Name].
    *   *Output/Note: Component file path.*
*   `[ ]` **3.3.3:** Add "Apply to [Integration Name]" Button (on output display).
    *   *Output/Note:*

### Mission: Wire Workflow with [Integration Name]

*   `[ ]` **3.4.1:** Frontend: Pull Context via [Integration Name] before generation.
    *   *Output/Note:*
*   `[ ]` **3.4.2:** Backend: Modify `/api/generateNicheOutput` to use integrated context.
    *   *Output/Note:*
*   `[ ]` **3.4.3:** Frontend: Wire "Apply" Button to Backend integration write module.
    *   *Output/Note:*

---

## 🔒 Phase 4: Lvl 4 - The Vault (Free vs Paid & Paywall)

**Boss Goal:** Gate features, push upgrades, capture leads.
**Founder's Vibe:** Show the value, then show the path to *more* value (paid).

### Mission: Feature Gating Implementation

*   `[ ]` **4.1.1:** Backend: User Role Check for `/api/generateNicheOutput`.
    *   *Output/Note:*
*   `[ ]` **4.1.2:** Backend: User Role Check for All Integration Endpoints.
    *   *Output/Note:*
*   `[ ]` **4.1.3:** Frontend: Hide/Disable Paid Features based on user role.
    *   *Output/Note:*
*   `[ ]` **4.1.4:** UI: Add Tooltips on Locked Features (value prop for upgrade).
    *   *Output/Note:*

### Mission: Free Tier Limits

*   `[ ]` **4.2.1:** Implement Usage Counter (DB, `users` table or `usage_logs`).
    *   *Output/Note: Schema changes link.*
*   `[ ]` **4.2.2:** Increment Counter for Free Niche Actions.
    *   *Output/Note:*
*   `[ ]` **4.2.3:** Enforce Backend Limits (e.g., daily/total generation for free users).
    *   *Output/Note:*

### Mission: Build Paywall & Upgrade UI

*   `[ ]` **4.3.1:** Design Paywall Modal/Page (Pricing, Niche ROI benefits).
    *   *Output/Note: Figma/design link.*
*   `[ ]` **4.3.2:** Implement Frontend Paywall Components.
    *   *Output/Note: File path.*
*   `[ ]` **4.3.3:** Trigger Paywall on Limit Reached / Locked Feature Click.
    *   *Output/Note:*

### Mission: Email Capture Flow

*   `[ ]` **4.4.1:** Build Email Input Modal UI.
    *   *Output/Note: File path.*
*   `[ ]` **4.4.2:** Trigger Modal after N Free Actions (e.g., 2 generates).
    *   *Output/Note:*
*   `[ ]` **4.4.3:** Backend: `/api/captureEmail` - Save Email & Grant Extra Free Credits.
    *   *Output/Note: Endpoint path.*

---

## 💾 Phase 5: Lvl 5 - The Hoard (Persistence & Library)

**Boss Goal:** Users save & reuse outputs, increasing stickiness.
**Founder's Vibe:** Let users build their personal AI treasure chest. Data for future RAG.

### Mission: Implement Save Output

*   `[ ]` **5.1.1:** Refine `niche_outputs` Schema (Apply migration: text, context, user_id, favorite, ts).
    *   *Output/Note:*
*   `[ ]` **5.1.2:** Create `/api/saveNicheOutput` Endpoint [Security, Free Limits Checked].
    *   *Output/Note: File path.*
*   `[ ]` **5.1.3:** Add Save Button/Icon to Frontend.
    *   *Output/Note:*

### Mission: Build Output Library

*   `[ ]` **5.2.1:** Create `/api/myNicheOutputs` Endpoint (Fetch for user, sort).
    *   *Output/Note: File path.*
*   `[ ]` **5.2.2:** Basic Library Page UI (e.g., `/library`).
    *   *Output/Note: File path.*
*   `[ ]` **5.2.3:** UI: List/Card Component for Saved Outputs.
    *   *Output/Note: File path.*
*   `[ ]` **5.2.4:** Add Basic Favorite Toggle (DB & Frontend).
    *   *Output/Note:*
*   `[ ]` **5.2.5:** Add Basic Search/Filter for Library (Frontend MVP, simple).
    *   *Output/Note:*

---

## 🎨 Phase 6: Lvl 6 - The Glow-Up (Core UX Polish)

**Boss Goal:** Make it look & feel professional.
**Founder's Vibe:** Clean, fast, intuitive. First impressions count.

### Mission: Responsiveness & Styling

*   `[ ]` **6.1.1:** UI Components Mobile Responsive (Check core workflow).
    *   *Output/Note: Tested on [Device(s)].*
*   `[ ]` **6.1.2:** Apply Consistent Color Palette & Typography (Tailwind theme fully used).
    *   *Output/Note:*

### Mission: Refine Workflow UI/UX

*   `[ ]` **6.2.1:** Add Global Loading States/Spinners for ALL async actions.
    *   *Output/Note:*
*   `[ ]` **6.2.2:** Implement Toast Notifications (Success/Error messages - e.g., `react-hot-toast`).
    *   *Output/Note:*
*   `[ ]` **6.2.3:** Improve Input Clarity (Labels, helper text, contextual placeholders).
    *   *Output/Note:*

### Mission: Implement Minimal Ads (if free tier has them)

*   `[ ]` **6.3.1:** Simple Ad Banner React Component Created.
    *   *Output/Note: File path.*
*   `[ ]` **6.3.2:** Ad Banner Conditional Placement for Free Users (Post-Output).
    *   *Output/Note:*

---

## 🔌 Phase 7: Lvl 7 - Into Their World (Chrome Extension MVP)

**Boss Goal:** Extension delivers core AI assist *inside* the Niche Tool.
**Founder's Vibe:** This is where we hook 'em. Zero friction AI.

### Mission: Extension Setup & Auth

*   `[ ]` **7.1.1:** Create Extension Project (Manifest V3, Webpack/Rollup build).
    *   *Output/Note: Build command working.*
*   `[ ]` **7.1.2:** Implement Auth Sync (Web App <> Extension via `chrome.storage.local` securely).
    *   *Output/Note: Token/status sync verified.*

### Mission: Context Detection & Popup ([1st Integration Name])

*   `[ ]` **7.2.1:** Content Script: Detect [1st Integration Name]'s relevant page URL/DOM.
    *   *Output/Note: Script injected on target pages.*
*   `[ ]` **7.2.2:** Content Script: Extract Key Context Data from page [Be Wary of DOM Changes].
    *   *Output/Note: Context extraction working for primary test cases.*
*   `[ ]` **7.2.3:** Build Basic Extension Popup UI (Mirror MVP inputs, show context).
    *   *Output/Note: Popup UI loads and shows context.*
*   `[ ]` **7.2.4:** Implement Message Passing: Page Context (CS) -> BG -> Popup.
    *   *Output/Note:*
*   `[ ]` **7.2.5:** Implement Popup logic to call backend `/api/generateNicheOutput`.
    *   *Output/Note:*

### Mission: Basic Apply/Inject ([1st Integration Name])

*   `[ ]` **7.3.1:** Implement Message Passing: Output (Popup) -> BG -> Content Script.
    *   *Output/Note:*
*   `[ ]` **7.3.2:** Content Script: Identify Target Input Field on [1st Integration Name]'s Page [Selector Strategy: ...].
    *   *Output/Note: Confirmed stable selectors for primary target field.*
*   `[ ]` **7.3.3:** Content Script: Inject Output & Trigger Events [Test This Hard!].
    *   *Output/Note: Injection works without breaking target page JS.*

---

## 💳 Phase 8: Lvl 8 - Cashflow Unlocked (Subscription & Billing)

**Boss Goal:** Users can pay us. Securely. Easily.
**Founder's Vibe:** Automated money printer setup. Lessgoo.

### Mission: Configure Payment Gateway

*   `[ ]` **8.1.1:** Setup Stripe/Razorpay Account & API Keys (securely stored in env).
    *   *Output/Note:*
*   `[ ]` **8.1.2:** Create Products/Plans in Payment Dashboard (as per pricing model).
    *   *Output/Note: Plan IDs documented.*

### Mission: Build Subscription Backend

*   `[ ]` **8.2.1:** Create `/api/create-checkout-session` Endpoint (for Stripe/Razorpay).
    *   *Output/Note: File path.*
*   `[ ]` **8.2.2:** Create `/api/manage-subscription` Endpoint (Stripe/Razorpay Customer Portal redirect).
    *   *Output/Note: File path.*

### Mission: Implement Webhook Handler

*   `[ ]` **8.3.1:** Create Secure Webhook Endpoint `/api/webhooks/[payment_gateway_name]`.
    *   *Output/Note: File path.*
*   `[ ]` **8.3.2:** Implement Webhook Signature Verification [SECURITY CHECK: PASSED].
    *   *Output/Note:*
*   `[ ]` **8.3.3:** Implement Logic to Update User Roles in DB (based on Subscription Events - created, updated, deleted).
    *   *Output/Note: Tested for key events.*

### Mission: Build Subscription UI

*   `[ ]` **8.4.1:** Create "Settings/Billing" Page (e.g., `/settings/billing`).
    *   *Output/Note: File path.*
*   `[ ]` **8.4.2:** UI: Display Current User Plan.
    *   *Output/Note:*
*   `[ ]` **8.4.3:** UI: Buttons/Links for Upgrade & Manage Subscription (triggers backend).
    *   *Output/Note:*

---

## 📈 Phase 9: Lvl 9 - Real World Grind (Beta Launch & Feedback Loop)

**Boss Goal:** Get it in Niche users' hands, learn, and iterate based on real data.
**Founder's Vibe:** This is where the real game begins. Data > opinions.

### Mission: Setup Monitoring & Analytics

*   `[ ]` **9.1.1:** Integrate Error Monitoring (Sentry/LogRocket) SDKs.
    *   *Output/Note: Test error reporting working.*
*   `[ ]` **9.1.2:** Setup Usage Analytics (Supabase/Firebase/GA4) - Track key Niche events.
    *   *Output/Note: Key events configured.*
*   `[ ]` **9.1.3:** Integrate LLM Cost Monitoring (Helicone/LangSmith) - Route LLM calls.
    *   *Output/Note: Costs showing in dashboard.*
*   `[ ]` **9.1.4:** Set up Basic Cost Alerts (LLM monitoring tool).
    *   *Output/Note:*

### Mission: Prepare for Beta

*   `[ ]` **9.2.1:** Create Niche-Focused Landing Page (simple for beta).
    *   *Output/Note: URL:*
*   `[ ]` **9.2.2:** Draft Onboarding Guide for Beta Users (MVP focus).
    *   *Output/Note: Link to guide.*
*   `[ ]` **9.2.3:** Prepare Feedback Channels (email, Slack/Discord, survey).
    *   *Output/Note: Channels created/configured.*

### Mission: Beta User Onboarding

*   `[ ]` **9.3.1:** Recruit Niche Beta Users (from interviewees, contacts).
    *   *Output/Note: Number of confirmed beta users:*
*   `[ ]` **9.3.2:** Grant Beta Access.
    *   *Output/Note:*

### Mission: Feedback & Iteration Loop

*   `[ ]` **9.4.1:** Implement Process: Regularly Review Errors, Analytics, Feedback.
    *   *Output/Note: Weekly review cadence set.*
*   `[ ]` **9.4.2:** Implement Process: Prioritize Bugs & Feature Requests (based on Niche Value).
    *   *Output/Note: Feedback Triage board link (Trello/Notion/etc.):*
*   `[ ]` **9.4.3:** Document Key Learnings & Plan Next Iteration (Update Roadmap/Backbone).
    *   *Output/Note: Next sprint priorities identified.*

