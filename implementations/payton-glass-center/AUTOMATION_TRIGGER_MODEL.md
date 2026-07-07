# Payton Glass Center Automation Trigger Model

Status: Draft
Blueprint AI Phase: Implementation Phase 1.12
Business: Payton Glass Center
Location: Louisville, Kentucky
Depends On: BUSINESS_INTAKE.md, CUSTOMER_JOURNEY.md, OFFER_CATALOG_DETAILED.md, GROUP_TOURS_SYSTEM_DETAILED.md, LOCAL_SEARCH_ALIGNMENT.md, WEBSITE_STRATEGY.md, WEBSITE_PAGE_MAP.md, WEBSITE_CONTENT_BLUEPRINT.md, LOCAL_LISTING_AUDIT.md, INQUIRY_FORM_MODEL.md, CRM_FIELD_MODEL.md

---

## 1. Purpose

This document defines the future automation trigger model for Payton Glass Center.

The goal is not to build automations yet.

The goal is to identify what business events should eventually trigger reminders, follow-ups, customer messages, CRM updates, internal tasks, review requests, pickup notices, rebooking reminders, and class interest workflows.

Automation should support the business model.

Automation should not replace business understanding.

---

## 2. Core Automation Principle

Do not automate confusion.

Before automation is built, the business must understand:

- The offer
- The customer journey
- The inquiry path
- The CRM fields
- The booking workflow
- The pickup workflow
- The review workflow
- The rebooking workflow

Automation should make a clear process easier.

It should not make an unclear process faster.

---

## 3. Automation Readiness Status

Payton Glass Center is not ready for final automation build-out yet.

Current status:

- Business intake documented
- Customer journey documented
- Offer catalog documented
- Group tours system documented
- Local search alignment documented
- Website strategy documented
- Website page map documented
- Website content blueprint documented
- Local listing audit documented
- Inquiry form model documented
- CRM field model documented

Next automation-related step:

Define the trigger model before choosing tools.

---

## 4. Main Automation Categories

Future automations may fall into these categories:

1. Inquiry intake
2. Internal notifications
3. Customer confirmation
4. Follow-up reminders
5. Booking confirmation
6. Deposit/payment reminders
7. Pre-visit instructions
8. Event preparation tasks
9. Pickup reminders
10. Review requests
11. Rebooking reminders
12. Class interest nurturing
13. Custom glass quote follow-up
14. Local listing maintenance
15. Content and marketing reminders

---

## 5. Trigger: New Inquiry Submitted

### Trigger Event

A customer submits an inquiry form on the website.

### Possible Inputs

- Name
- Email
- Phone
- Offer interest
- Group type
- Organization
- Participant count
- Preferred date
- Message
- Referral source
- Page source

### Future Actions

- Create CRM contact
- Create CRM inquiry
- Tag inquiry type
- Send internal notification
- Send customer confirmation
- Create follow-up task
- Route based on offer interest

### Priority

High

### Notes

This is likely the first automation to build later.

Do not build until the form and CRM tool are selected.

---

## 6. Trigger: New Phone Inquiry Logged

### Trigger Event

A phone inquiry is manually entered into the CRM.

### Future Actions

- Create contact
- Create inquiry
- Set inquiry source as Phone Call
- Assign follow-up status
- Create next action task

### Priority

High

### Notes

Not every inquiry will come from the website.

The CRM must allow manual entry.

---

## 7. Trigger: Group Tour Inquiry Received

### Trigger Event

Inquiry type equals Group Tour.

### Future Actions

- Apply Group Tour tag
- Create group tour follow-up task
- Send group tour information if appropriate
- Request missing group details if needed
- Set status to Needs Response
- Start group tour inquiry workflow

### Possible Customer Message

Thank you for asking about a group tour at Payton Glass Center. To help us respond accurately, please include your group size, age range, preferred date and time, and the type of activity you are interested in.

### Priority

High

---

## 8. Trigger: Field Trip Inquiry Received

### Trigger Event

Inquiry type equals Field Trip.

### Future Actions

- Apply Field Trip tag
- Create teacher/group organizer follow-up task
- Request school name, grade level, student count, and preferred date if missing
- Add to education/group segment
- Create possible annual rebooking opportunity after completion

### Priority

High

---

## 9. Trigger: Fused Glass Workshop Inquiry Received

### Trigger Event

Inquiry type equals Fused Glass Workshop.

### Future Actions

- Apply Fused Glass tag
- Create workshop follow-up task
- Ask for participant count, age range, preferred date, and project interest if missing
- Prepare pickup reminder workflow if booking is completed

### Priority

Medium to High

---

## 10. Trigger: Hands-On Torch Experience Inquiry Received

### Trigger Event

Inquiry type equals Hands-On Torch Experience.

### Future Actions

- Apply Hands-On Torch tag
- Create follow-up task
- Ask for participant count, age range, preferred date, and experience level if missing
- Send safety/preparation information after booking
- Add future class interest tag if appropriate

### Priority

Medium to High

---

## 11. Trigger: Private Event or Birthday Inquiry Received

### Trigger Event

Inquiry type equals Private Event or Birthday Activity.

### Future Actions

- Apply Private Event or Birthday tag
- Create event planning follow-up task
- Ask for group size, age range, preferred date, activity interest, and event type if missing
- Create possible birthday anniversary reminder after completion if appropriate

### Priority

Medium to High

---

## 12. Trigger: Class Interest Inquiry Received

### Trigger Event

Inquiry type equals Class Interest.

### Future Actions

- Add contact to class interest list
- Tag by interest area
- Tag by skill level
- Tag by preferred schedule
- Send class interest confirmation
- Notify when future classes are announced

### Priority

Medium

### Notes

This is important for future evening, weekend, one-day, two-day, and multi-session class offerings.

---

## 13. Trigger: Custom Glass Inquiry Received

### Trigger Event

Inquiry type equals Custom Glass.

### Future Actions

- Create custom glass request record
- Ask for reference photos if missing
- Ask for size, color, deadline, and budget if needed
- Create feasibility review task
- Create quote follow-up task

### Priority

Medium

---

## 14. Trigger: Date Confirmed

### Trigger Event

Inquiry or event status changes to Date Confirmed.

### Future Actions

- Create event/booking record
- Send booking confirmation
- Create pre-visit instruction task
- Create material preparation task if needed
- Create payment/deposit task if applicable

### Priority

High

---

## 15. Trigger: Deposit Needed

### Trigger Event

Event status changes to Deposit Needed.

### Future Actions

- Create deposit reminder task
- Send deposit instructions if automation is appropriate
- Set follow-up date
- Keep event as tentative until deposit is handled if policy requires it

### Priority

Medium

### Notes

Only automate this after the deposit policy is clearly defined.

---

## 16. Trigger: Deposit Paid

### Trigger Event

Deposit Paid field changes to yes.

### Future Actions

- Update event status
- Send confirmation if appropriate
- Create pre-visit information task
- Mark booking as stronger/confirmed

### Priority

Medium

---

## 17. Trigger: Pre-Visit Window

### Trigger Event

Event date is approaching.

Possible timing:

- 7 days before event
- 3 days before event
- 1 day before event

### Future Actions

- Send pre-visit instructions
- Confirm group size
- Confirm arrival time
- Confirm activity
- Include parking/address information
- Include clothing/safety notes if needed
- Include pickup expectations if needed

### Priority

High

### Notes

The timing should match the real workflow.

---

## 18. Trigger: Event Completed

### Trigger Event

Event status changes to Completed.

### Future Actions

- Create pickup task if needed
- Create review request task
- Create rebooking opportunity if group or organization
- Mark inquiry as completed/closed won
- Update contact last visit date
- Update organization last visit date
- Add notes about satisfaction or issues

### Priority

High

---

## 19. Trigger: Pickup Required

### Trigger Event

Pickup Required field changes to yes.

### Future Actions

- Create pickup task
- Set expected ready date
- Track item status
- Notify customer when ready
- Send reminder if not picked up

### Priority

High

---

## 20. Trigger: Item Ready for Pickup

### Trigger Event

Pickup status changes to Ready for Pickup.

### Future Actions

- Send pickup notification
- Create pickup reminder task
- Update pickup status to Customer Notified
- Record notification date

### Priority

High

---

## 21. Trigger: Pickup Overdue

### Trigger Event

Pickup item remains unclaimed after defined period.

Possible timing:

- 7 days after ready date
- 14 days after ready date
- 30 days after ready date

### Future Actions

- Send reminder
- Create internal follow-up task
- Mark as overdue
- Apply unclaimed item policy if defined

### Priority

Medium

### Notes

Do not automate final abandonment decisions until policy is defined.

---

## 22. Trigger: Review Request Ready

### Trigger Event

Event completed and customer had a positive or normal experience.

### Future Actions

- Send Google review request
- Create review request record
- Mark review request sent
- Track whether completed if known

### Priority

High

### Notes

Review requests should be respectful, simple, and compliant with platform policies.

Do not offer improper incentives.

---

## 23. Trigger: Rebooking Opportunity Created

### Trigger Event

Completed group event, school field trip, corporate event, senior group visit, or repeatable group visit.

### Future Actions

- Create rebooking opportunity
- Set suggested follow-up date
- Tag organization
- Create reminder near next likely booking window

### Priority

Medium to High

### Examples

- School field trip follow-up next school year
- Homeschool group follow-up next semester
- Corporate group follow-up next year
- Birthday reminder next year
- Senior group seasonal follow-up

---

## 24. Trigger: Class Announcement Ready

### Trigger Event

New class or workshop date is ready to promote.

### Future Actions

- Notify class interest list
- Segment by interest area
- Segment by preferred schedule
- Post to website if needed
- Create social media/content tasks

### Priority

Medium

---

## 25. Trigger: Local Listing Review Due

### Trigger Event

Scheduled recurring review of business listings.

Possible schedule:

- Monthly for Google Business Profile
- Quarterly for Bing Places
- Quarterly for Apple Business Connect
- Quarterly for directory consistency

### Future Actions

- Review hours
- Review services
- Review photos
- Review Q&A
- Review reviews
- Check for duplicate listings
- Update posts or media if needed

### Priority

Medium

---

## 26. Trigger: New Review Received

### Trigger Event

New review appears on Google, Facebook, Yelp, TripAdvisor, or another platform.

### Future Actions

- Notify owner/staff
- Record review if useful
- Respond if appropriate
- Identify themes
- Flag strong testimonial candidates
- Flag negative review for attention

### Priority

Medium

---

## 27. Trigger: Website Content Update Needed

### Trigger Event

A business detail changes.

Examples:

- New offer
- Changed price
- Changed hours
- Changed age limit
- Changed group capacity
- Changed booking policy
- New class launch
- New pickup policy
- New photos

### Future Actions

- Update website
- Update Google Business Profile if relevant
- Update Bing and Apple listings if relevant
- Update FAQ if relevant
- Update CRM fields if relevant
- Update automation messages if relevant

### Priority

High when business facts change

---

## 28. Trigger Priority Ranking

Recommended first automation priorities:

1. New inquiry notification
2. Customer inquiry confirmation
3. Inquiry type tagging
4. Follow-up task creation
5. Booking confirmation
6. Pre-visit instruction reminder
7. Pickup reminder
8. Review request
9. Rebooking reminder
10. Class interest list
11. Local listing review reminder
12. Content update reminder

---

## 29. Minimum Viable Automation Set

The first useful automation set should include:

### Automation 1 — New Inquiry Intake

When a form is submitted:

- Notify owner/staff
- Create CRM inquiry
- Send customer confirmation

### Automation 2 — Follow-Up Reminder

When an inquiry is marked Needs Response or Waiting on Customer:

- Create reminder task
- Keep inquiry visible

### Automation 3 — Pre-Visit Reminder

When an event is confirmed:

- Remind staff to send pre-visit instructions
- Later send automatically if ready

### Automation 4 — Pickup Reminder

When item is ready:

- Notify customer
- Track pickup status

### Automation 5 — Review Request

After completed visit:

- Send review request or create task to send manually

Do not build more than this until the first system is working.

---

## 30. Automation Risk Areas

Risks to avoid:

- Sending wrong details automatically
- Sending pricing before it is finalized
- Sending booking confirmation before date is actually confirmed
- Sending deposit reminders without a defined deposit policy
- Sending pickup reminders before items are ready
- Sending review requests after a bad experience
- Over-automating personal customer interactions
- Creating too many reminders
- Building automations before CRM statuses are used consistently
- Connecting tools before the workflow is clear

---

## 31. Human Approval Points

Some actions should require human approval, at least at first:

- Final booking confirmation
- Custom glass feasibility
- Custom glass quote
- Deposit/payment issue
- Cancellation or rescheduling
- Negative review response
- Unclaimed pickup decision
- Large group capacity approval
- Special needs/accommodation handling
- Price exceptions
- Private event custom requests

Automation should assist, not override judgment.

---

## 32. Tool Selection Notes

Do not select automation tools yet.

This model can later be implemented through:

- Website form tool
- CRM automation
- Email automation
- Zapier/Make/n8n
- Airtable automation
- Google Sheets automation
- Booking platform automation
- Custom app logic
- AI agent workflow later

Tool choice should follow the process, not the other way around.

---

## 33. Open Questions

Owner input needed later:

- Who receives inquiry notifications?
- What response time should customers expect?
- Should customers get automatic replies immediately?
- What details should be included in group tour replies?
- What is the deposit policy?
- What is the cancellation policy?
- What is the pickup timeline?
- How should review requests be sent?
- Should text messaging be used?
- Should automation create calendar events?
- Should automation connect to email marketing?
- What CRM or database will be used first?
- Which automations must stay manual at first?
- Which automations would save the most time immediately?

---

## 34. Blueprint AI Notes

This document validates Blueprint AI by turning the business model, customer journey, inquiry form, and CRM field model into an automation-ready operating system.

Automation should be treated as the final layer after clarity.

The order is:

1. Understand the business
2. Map the customer journey
3. Define offers
4. Document workflows
5. Structure the website
6. Align local search
7. Model the form
8. Model the CRM
9. Define automation triggers
10. Build only the automations that serve the real workflow
