- Test case


---
## 2026-06-22 — product_design
**Question:** Test question

**Model Answer:** Test answer

**My Notes:** Test notes

**What I Missed:** Test reflection

---
## 2026-06-22 — product_design
**Question:** Test question

**Model Answer:** Test answer

**My Notes:** Test notes

**What I Missed:** Test reflection

---
## 2026-06-22 — product_design
**Question:** Test question

**Model Answer:** Test answer

**My Notes:** Test notes

**What I Missed:** Test reflection

---
## 2026-06-22 — product_design
**Question:** Design an onboarding experience for a professional-grade creative tool (like Figma or Adobe Premiere) that significantly reduces "time-to-first-mastery" for a user migrating from a legacy competitor, specifically addressing the friction caused by deeply ingrained muscle memory and disparate UI paradigms.

**Model Answer:** Design an end-to-end experience for a feature that allows users to seamlessly split and trade fractional ownership of physical high-value assets—such as fine art, classic cars, or luxury watches—within a peer-to-peer marketplace, ensuring regulatory compliance and liquidity.

**My Notes:** user: potentially UX team
pain points: high switching cost becasue they are used to using the legacy tool
solution: built an AI onboarding tool -> user tells the AI that i currently use this tool. in this i could do this using step xyz, AI tool gives you how to do it in this new tool
metrics: measure the adoption, outcome: switch decisions

**What I Missed:** i could do segmentation better, more solutions.

---
## 2026-06-23 — product_design
**Question:** Design a feature for a ride-sharing platform that allows users to optimize for "total trip utility" rather than just speed or cost, specifically for users commuting between suburban residential zones and dense urban office centers who currently struggle with the trade-offs between last-mile transit connectivity and door-to-door comfort.

**Model Answer:** Design a feature for a high-frequency ride-sharing app that dynamically reconciles the conflicting needs of passengers wanting lower prices and drivers wanting higher earnings during periods of extreme supply-demand imbalance, while ensuring the platform maintains long-term marketplace health and brand trust.

**My Notes:** users: daily commuters
problems: either take door-to-door cab: expensive but comfortable and fast
or take public transport: cheap but discomfort and slow
solution: can we find a middle ground?
1. schedule pool rides: tells the app that i want to go from A -> B at 6PM. App automatically creates a pool for optimal riders
2. have a home to metro option recurring booking and metro to office recurring booking on the app. fixed price.
3. if someone is driving, they can tell the app ad-hoc and they can give you some co-passengers/

pick the first one.
metrics: repeat users, ARPU, unit economics of platform

**What I Missed:** need to fix the model answer

---
## 2026-06-24 — product_design
**Question:** Design a system for a peer-to-peer marketplace (such as eBay or Vinted) that proactively mitigates "transactional anxiety" for high-value items, specifically addressing the trust deficit between novice sellers and expert collectors where the primary points of friction are subjective condition grading, shipping liability, and the risk of fraudulent returns.

**Model Answer:** Design a solution for a collaborative document editing platform that enables teams to maintain "contextual continuity" when transitioning from asynchronous drafting to real-time sync meetings, specifically addressing the friction where information density in long-form documents leads to fragmented decision-making and loss of alignment during live discussions.

**My Notes:** stakeholder: buyer, seller, platform
problem: for high value items, both buyer and seller can't trust each other easily. 
solution: 1. the platform act as a trust (buyer pays money to the platform and the platform holds it, and pays it to the seller as soon as the product is received).
2. the platform arranges the quality checks and the delivery.
3. the platform ensure AI based quality checks.

solution 1 -> limited liability and easy to build, high impact

**What I Missed:** metrics and edge cases

---
## 2026-06-25 — product_design
**Question:** Design a collaborative decision-making interface for a project management suite that addresses "contextual drift" in cross-functional teams, specifically solving for the friction where asynchronous updates in a project plan cause misalignment between engineering, product, and stakeholders, despite all parties having access to the same centralized source of truth.

**Model Answer:** To address **contextual drift**, we must shift the paradigm from "a shared document" to "a shared decision trail." The problem isn't the lack of information; it’s the lack of *intent* behind the changes.

### 1. User Insight
When an engineer or PM updates a project plan asynchronously, they are often focused on the *output* (e.g., changing a date) rather than the *impact* on the stakeholder's mental model. Stakeholders notice the change, lose trust in the timeline, and initiate a "communication tax"—back-and-forth threads to understand the "why"—which creates friction and delays.

### 2. Problem Definition
The centralized source of truth (the plan) fails because it is **stateless**. It shows the *current* state but hides the *evolution* of the decision. We need to bridge the gap between "the change" and "the context" to prevent misalignment.

### 3. Proposed Solution: The "Decision-Gate & Contextual-Diff" Feature
I propose a two-part UI intervention within the project suite:

*   **Intent-Based Change Request:** When a user moves a task or changes a status/scope, a lightweight "Why this change?" modal triggers automatically. It offers pre-filled tags (e.g., "Dependency Shift," "Scope Creep," "Resource Constraint"). The user’s input becomes a mandatory "comment-as-change-log."
*   **The "Delta-View" Sidebar:** Instead of a generic notification feed, the UI includes a "Delta-View" dashboard. This highlights what changed in the last 24 hours in the user’s specific lane. It visually pairs the **old state vs. new state** with the **attached "Why" context** pinned directly to the element. 

### 4. Trade-offs
*   **Friction vs. Clarity:** Requiring an explanation for every change adds a "friction tax" to the contributor. 
    *   *Mitigation:* Use AI-suggested justifications based on previous comments or Slack/Jira history so users can click to confirm rather than write.
*   **Notification Fatigue:** If every minor change prompts a "Delta," users will tune it out.
    *   *Mitigation:* Use "Smart Grouping." Only alert stakeholders if the change impacts their specific KPIs or critical path dependencies.

### 5. Success Metrics
*   **Primary Metric: "Sync-Time Latency":** The time elapsed between a project plan update and the stakeholder’s acknowledgment/approval of the change. A successful product should reduce this time.
*   **Secondary Metric: "Communication Tax Ratio":** The volume of Slack/email threads initiated regarding "Why did X change?" compared to the number of changes made in the platform. A downward trend indicates better contextual clarity.
*   **Qualitative Metric:** Sentiment score from periodic surveys asking users: *"Do you feel surprised by plan changes?"* (Goal: Reduce "surprisal" events).

***

### PM Interviewer Tip:
*If asked for a "moonshot" feature:* I would suggest a **"Simulation Mode."** Before an engineer hits "Save" on a major timeline shift, they can toggle "Simulate Change." The UI would highlight exactly which stakeholder KPIs will turn "red" or "at-risk" before the change is committed, forcing proactive alignment rather than reactive fixing.

**My Notes:** user, problem, solution, metrics

**What I Missed:** reflection test