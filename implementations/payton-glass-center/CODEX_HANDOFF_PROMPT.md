# Codex Handoff Prompt

Status: Draft
Blueprint AI Phase: Implementation Phase 4
Business: Payton Glass Center
Location: Louisville, Kentucky
Phase Focus: Controlled Codex build prompt preparation
Depends On:
- AGENT_BUILD_HANDOFF.md
- FIRST_BUILD_TECHNICAL_BRIEF.md
- BUILD_PREPARATION_CHECKLIST.md
- WEBSITE_ASSET_CHECKLIST.md
- WEBSITE_BUILD_DECISION.md
- WEBSITE_BUILD_PLAN.md
- FIRST_BUILD_SCOPE.md
- WEBSITE_PAGE_MAP.md
- WEBSITE_CONTENT_BLUEPRINT.md
- WEBSITE_COPY_DRAFTS.md
- INQUIRY_FORM_SPEC.md
- EXECUTION_READINESS_CHECKLIST.md
- PHASE_3_SUMMARY.md

---

## 1. Purpose

This file contains the controlled handoff prompt to use with Codex when Payton Glass Center is ready for the first website build.

This prompt is intentionally constrained.

It is not a general request to “make a website.”

It tells Codex what to read, what to build, what to avoid, and where to stop.

---

## 2. When to Use This Prompt

Use this prompt only after Phase 4 preparation files are complete and committed.

Before using this prompt, confirm:

- BUILD_PREPARATION_CHECKLIST.md exists
- WEBSITE_ASSET_CHECKLIST.md exists
- FIRST_BUILD_TECHNICAL_BRIEF.md exists
- AGENT_BUILD_HANDOFF.md exists
- Owner has decided to continue with an Astro-based first build or has documented a different decision
- The repo is clean
- Codex is being asked to prepare or build the first website version only

---

## 3. Codex Role

Codex should act as a careful implementation assistant.

Codex should not act as:

- Business strategist
- Brand reinvention agent
- Booking system architect
- CRM architect
- Ecommerce builder
- Listing manager
- Public launch agent
- DNS manager
- Marketing automation builder

Codex’s job is to follow the approved strategy and create a clean technical first build.

---

## 4. Required Codex Behavior

Codex must:

- Read the required files before building
- Summarize the intended build plan before creating files
- List the files it expects to create or modify
- Build only the approved first version
- Preserve Payton Glass Center’s real business identity
- Prioritize group tours plus activity
- Keep the build simple
- Avoid premature automation
- Stop before public launch
- Clearly document any missing owner decisions

---

## 5. Do Not Let Codex Add

Codex must not add:

- Online booking
- Ecommerce
- Payment automation
- Full CRM integration
- AI customer replies
- Public chatbot
- Listing automation
- Public listing changes
- DNS changes
- Customer login
- Gift card automation
- Class calendar system
- Marketing automation
- Complex scheduling logic
- Unsupported policies
- Fake testimonials
- Fake reviews
- Fake pricing
- Fake hours

---

## 6. Copyable Codex Prompt

Use the following prompt when opening a new Codex build session.

```text id="h3xq6p"
You are helping build the first website for Payton Glass Center from the Blueprint AI implementation repository.

Repository:
C:\Projects\Blueprint-AI

Business:
Payton Glass Center is a working glass art studio and hands-on glass experience center in Louisville, Kentucky.

Primary business priority:
Group tours plus activity are a major revenue driver and must be treated as a primary conversion path.

First build goal:
Create a clean first website version that clearly explains Payton Glass Center, prioritizes group tours plus activity, explains hands-on glass experiences, supports local search clarity, supports AEO / AI answer readiness, and captures inquiries through a simple form.

Preferred technical direction:
Astro-based website unless the owner explicitly changes the decision.

Before creating or editing files, read these files:

1. implementations/payton-glass-center/AGENT_BUILD_HANDOFF.md
2. implementations/payton-glass-center/FIRST_BUILD_TECHNICAL_BRIEF.md
3. implementations/payton-glass-center/BUILD_PREPARATION_CHECKLIST.md
4. implementations/payton-glass-center/WEBSITE_ASSET_CHECKLIST.md
5. implementations/payton-glass-center/WEBSITE_BUILD_DECISION.md
6. implementations/payton-glass-center/WEBSITE_BUILD_PLAN.md
7. implementations/payton-glass-center/FIRST_BUILD_SCOPE.md
8. implementations/payton-glass-center/WEBSITE_PAGE_MAP.md
9. implementations/payton-glass-center/WEBSITE_CONTENT_BLUEPRINT.md
10. implementations/payton-glass-center/WEBSITE_COPY_DRAFTS.md
11. implementations/payton-glass-center/INQUIRY_FORM_SPEC.md
12. implementations/payton-glass-center/EXECUTION_READINESS_CHECKLIST.md
13. implementations/payton-glass-center/PHASE_3_SUMMARY.md

Helpful supporting context:

- implementations/payton-glass-center/BUSINESS_PROFILE.md
- implementations/payton-glass-center/OFFER_MAP.md
- implementations/payton-glass-center/CUSTOMER_JOURNEY.md
- implementations/payton-glass-center/GROUP_TOURS_SYSTEM_DETAILED.md
- implementations/payton-glass-center/LOCAL_SEARCH_ALIGNMENT.md
- implementations/payton-glass-center/LOCAL_LISTING_AUDIT.md
- implementations/payton-glass-center/CRM_FIRST_STEP_DECISION.md

Build only the approved first website version.

Approved first build pages:

- /
- /group-tours/
- /hands-on-glass/
- /fused-glass/
- /gallery/
- /custom-glass/
- /about/
- /contact/

Optional pages only if simple:

- /field-trips/
- /private-groups/
- /corporate-events/
- /classes/
- /faq/

Do not build or add:

- Online booking
- Ecommerce
- Payment collection
- Customer accounts
- Full CRM integration
- AI customer replies
- Public AI chatbot
- Listing automation
- Public listing updates
- DNS changes
- Marketing automation
- Gift card automation
- Class calendar system
- Advanced scheduling logic
- Unsupported policies
- Fake testimonials
- Fake reviews
- Fake pricing
- Fake business hours

Before creating files, respond with:

1. A short summary of the build plan
2. The exact files and folders you expect to create or modify
3. Any assumptions you are making
4. Any missing information that should be marked as placeholder instead of invented

After that, proceed one controlled step at a time.

The first technical goal is to create a clean Astro-based first website foundation that can be previewed locally but not published live without owner approval.
