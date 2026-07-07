# Payton Glass Center CRM Field Model

Status: Draft
Blueprint AI Phase: Implementation Phase 1.11
Business: Payton Glass Center
Location: Louisville, Kentucky
Depends On: BUSINESS_INTAKE.md, CUSTOMER_JOURNEY.md, OFFER_CATALOG_DETAILED.md, GROUP_TOURS_SYSTEM_DETAILED.md, LOCAL_SEARCH_ALIGNMENT.md, WEBSITE_STRATEGY.md, WEBSITE_PAGE_MAP.md, WEBSITE_CONTENT_BLUEPRINT.md, LOCAL_LISTING_AUDIT.md, INQUIRY_FORM_MODEL.md

---

## 1. Purpose

This document defines the future CRM field model for Payton Glass Center.

The goal is not to choose CRM software yet.

The goal is to define what the business needs to track before selecting or building any CRM, automation, booking, or follow-up system.

A good CRM for Payton Glass Center should help track:

- Contacts
- Organizations
- Inquiries
- Group tours
- Field trips
- Workshops
- Hands-on experiences
- Private events
- Class interest
- Custom glass requests
- Pickup tasks
- Follow-up status
- Reviews
- Referrals
- Rebooking opportunities
- Source tracking

---

## 2. Core CRM Principle

The CRM should reflect the real business model.

Do not start with software features.

Start with the business reality:

- A person contacts the studio.
- They are interested in a specific offer.
- Some inquiries involve groups or organizations.
- Some inquiries become scheduled visits.
- Some visits create pickup tasks.
- Some customers should receive review requests.
- Some groups should be followed up with later.
- Some customers may become class students, collectors, repeat visitors, or referral sources.

The CRM should make these paths visible and manageable.

---

## 3. Recommended CRM Objects

The CRM should eventually support these object types or record types:

1. Contact
2. Organization
3. Inquiry
4. Event / Booking
5. Offer Interest
6. Activity / Project
7. Pickup Task
8. Follow-Up Task
9. Review Request
10. Rebooking Opportunity
11. Custom Glass Request
12. Class Interest Record

Depending on the CRM tool, these may be separate objects, tables, tags, pipelines, or custom fields.

---

## 4. Contact Object

### Purpose

Tracks individual people who interact with Payton Glass Center.

### Example Contacts

- Parent
- Teacher
- School coordinator
- Corporate organizer
- Birthday planner
- Individual participant
- Custom glass customer
- Class interest lead
- Gift buyer
- Returning customer

### Recommended Contact Fields

| Field | Type | Purpose |
|---|---|---|
| First Name | Text | Contact identity |
| Last Name | Text | Contact identity |
| Full Name | Text | Display name |
| Email | Email | Contact method |
| Phone | Phone | Contact method |
| Preferred Contact Method | Dropdown | Email, phone, text |
| SMS Consent | Checkbox | Future texting compliance |
| Customer Type | Dropdown | Segment |
| Primary Offer Interest | Dropdown | Main interest |
| Referral Source | Dropdown | Where they came from |
| First Inquiry Date | Date | Initial contact |
| Last Contact Date | Date | Recent interaction |
| Notes | Long Text | Human context |
| Tags | Multi-select | Flexible grouping |

### Customer Type Options

- Individual
- Family
- Parent
- Teacher
- School Coordinator
- Homeschool Organizer
- Scout / Youth Leader
- Senior Group Organizer
- Corporate Organizer
- Church Group Organizer
- Birthday Organizer
- Tourist
- Artist / Creative Adult
- Gift Buyer
- Custom Glass Customer
- Returning Customer
- Other

---

## 5. Organization Object

### Purpose

Tracks schools, companies, churches, community groups, clubs, and organizations.

### Example Organizations

- School
- Homeschool group
- Scout troop
- Senior center
- Corporation
- Church
- Tourist group
- Community organization
- Club
- Nonprofit

### Recommended Organization Fields

| Field | Type | Purpose |
|---|---|---|
| Organization Name | Text | Group identity |
| Organization Type | Dropdown | Segment |
| Main Contact | Linked Contact | Primary person |
| Phone | Phone | Organization phone if different |
| Email | Email | Organization email if different |
| Address | Text | Optional |
| Website | URL | Optional |
| Notes | Long Text | Context |
| Rebooking Window | Dropdown/Date | Future follow-up |
| Last Visit Date | Date | History |
| Total Visits | Number | Relationship value |

### Organization Type Options

- School
- Homeschool Group
- Scout / Youth Group
- Senior Group
- Corporate Team
- Church Group
- Tourist Group
- Birthday Group
- Club
- Community Organization
- Nonprofit
- Other

---

## 6. Inquiry Object

### Purpose

Tracks each incoming request.

A single contact may have multiple inquiries over time.

### Example Inquiries

- Group tour inquiry
- Field trip inquiry
- Fused glass workshop inquiry
- Hands-on torch inquiry
- Birthday inquiry
- Private event inquiry
- Class interest inquiry
- Custom glass inquiry
- General question

### Recommended Inquiry Fields

| Field | Type | Purpose |
|---|---|---|
| Inquiry ID | Auto/Text | Unique record |
| Contact | Linked Contact | Person asking |
| Organization | Linked Organization | Group if applicable |
| Inquiry Type | Dropdown | Offer interest |
| Inquiry Source | Dropdown | Where it came from |
| Page Source | Dropdown | Website page |
| Referral Source | Dropdown | Self-reported source |
| Inquiry Date | Date/Time | When received |
| Status | Dropdown | Pipeline status |
| Priority | Dropdown | Response priority |
| Preferred Date | Date | Scheduling |
| Preferred Time | Text/Dropdown | Scheduling |
| Backup Date | Date | Scheduling |
| Flexible Dates | Checkbox | Scheduling |
| Participant Count | Number | Capacity |
| Non-Participant Count | Number | Chaperones/guests |
| Age Range / Grade Level | Text | Suitability |
| Message | Long Text | Customer request |
| Special Notes | Long Text | Accessibility/details |
| Next Follow-Up Date | Date | Follow-up |
| Assigned To | User/Text | Owner |
| Outcome | Dropdown | Result |

### Inquiry Type Options

- Group Tour
- Field Trip
- Fused Glass Workshop
- Hands-On Torch Experience
- Private Event
- Birthday Activity
- Class Interest
- Custom Glass
- Glass Art / Gift
- Demonstration / Studio Visit
- General Question

### Inquiry Status Options

- New Inquiry
- Needs Response
- Waiting on Customer
- Details Sent
- Quote Sent
- Date Requested
- Date Confirmed
- Deposit Needed
- Deposit Paid
- Confirmed
- Completed
- Pickup Pending
- Review Requested
- Rebooking Opportunity
- Closed Won
- Closed Lost
- Canceled
- Rescheduled

### Inquiry Source Options

- Website Form
- Phone Call
- Email
- Google Business Profile
- Google Maps
- Bing
- Apple Maps
- Facebook
- Instagram
- YouTube
- AI Search
- Walk-In
- Referral
- Returning Customer
- Other

### Outcome Options

- Booked
- Not Booked
- Waiting
- Referred Elsewhere
- Future Interest
- Duplicate
- Not a Fit
- Unknown

---

## 7. Event / Booking Object

### Purpose

Tracks scheduled visits, tours, workshops, and events.

An inquiry becomes an event or booking when a date/time is confirmed.

### Example Events

- School field trip
- Group tour
- Birthday glass activity
- Corporate team outing
- Fused glass workshop
- Hands-on torch session
- Private event
- Demonstration visit

### Recommended Event Fields

| Field | Type | Purpose |
|---|---|---|
| Event ID | Auto/Text | Unique event |
| Event Name | Text | Display name |
| Contact | Linked Contact | Organizer |
| Organization | Linked Organization | Group |
| Related Inquiry | Linked Inquiry | Source |
| Event Type | Dropdown | Offer/category |
| Event Status | Dropdown | Stage |
| Event Date | Date | Scheduled date |
| Start Time | Time | Schedule |
| End Time | Time | Schedule |
| Participant Count | Number | Planning |
| Non-Participant Count | Number | Chaperones/guests |
| Age Range / Grade Level | Text | Suitability |
| Activity Selected | Dropdown/Text | What they are doing |
| Price / Quote | Currency | Expected amount |
| Deposit Required | Checkbox | Payment |
| Deposit Paid | Checkbox | Payment |
| Balance Due | Currency | Payment |
| Payment Status | Dropdown | Payment tracking |
| Pre-Visit Info Sent | Checkbox | Process |
| Pickup Required | Checkbox | Process |
| Pickup Status | Dropdown | Process |
| Review Requested | Checkbox | Follow-up |
| Rebooking Potential | Dropdown | Future value |
| Internal Notes | Long Text | Staff context |

### Event Type Options

- Group Tour
- Field Trip
- Fused Glass Workshop
- Hands-On Torch Experience
- Private Event
- Birthday Activity
- Demonstration / Studio Visit
- Class
- Other

### Event Status Options

- Tentative
- Confirmed
- Deposit Needed
- Deposit Paid
- Pre-Visit Info Sent
- Completed
- Pickup Pending
- Review Requested
- Closed
- Canceled
- Rescheduled
- No-Show

### Payment Status Options

- Not Required
- Quote Sent
- Deposit Needed
- Deposit Paid
- Balance Due
- Paid in Full
- Refunded
- Canceled

---

## 8. Offer Interest Object / Field

### Purpose

Tracks what the customer is interested in, even if they do not book immediately.

### Recommended Fields

| Field | Type | Purpose |
|---|---|---|
| Offer Interest | Dropdown | Main offer |
| Secondary Interest | Multi-select | Additional offers |
| Interest Level | Dropdown | Strength |
| Future Follow-Up Date | Date | Nurture |
| Notes | Long Text | Context |

### Interest Level Options

- High
- Medium
- Low
- Future Interest
- Researching
- Unknown

---

## 9. Activity / Project Field Model

### Purpose

Tracks what participants are making or doing.

This may become important for pricing, pickup, capacity, and repeat offers.

### Recommended Fields

| Field | Type | Purpose |
|---|---|---|
| Activity Type | Dropdown | General activity |
| Project Name | Text/Dropdown | Specific project |
| Quantity | Number | Number of pieces |
| Requires Kiln Firing | Checkbox | Process |
| Requires Cooling | Checkbox | Process |
| Pickup Required | Checkbox | Process |
| Pickup Date | Date | Process |
| Notes | Long Text | Details |

### Activity Type Options

- Fused Glass
- Torch Experience
- Demonstration
- Group Tour Activity
- Custom Glass
- Class Project
- Retail / Gift
- Other

---

## 10. Pickup Task Object

### Purpose

Tracks pieces that need cooling, firing, labeling, pickup, or shipping.

### Recommended Pickup Fields

| Field | Type | Purpose |
|---|---|---|
| Pickup ID | Auto/Text | Unique record |
| Contact | Linked Contact | Customer |
| Related Event | Linked Event | Source event |
| Related Activity | Linked Activity | Project |
| Item Description | Text | What it is |
| Quantity | Number | Pieces |
| Pickup Status | Dropdown | Stage |
| Ready Date | Date | When ready |
| Customer Notified | Checkbox | Communication |
| Notification Date | Date | Communication |
| Pickup Date | Date | Completed date |
| Shipping Needed | Checkbox | Alternative |
| Shipping Address | Text | Shipping |
| Notes | Long Text | Context |

### Pickup Status Options

- Not Required
- Pending Cooling
- Pending Firing
- In Kiln
- Ready for Pickup
- Customer Notified
- Picked Up
- Shipped
- Overdue
- Abandoned / Unclaimed
- Issue / Broken

---

## 11. Follow-Up Task Object

### Purpose

Tracks what needs to happen next.

### Recommended Fields

| Field | Type | Purpose |
|---|---|---|
| Task Name | Text | Action |
| Related Contact | Linked Contact | Person |
| Related Inquiry | Linked Inquiry | Inquiry |
| Related Event | Linked Event | Booking |
| Task Type | Dropdown | Kind of action |
| Due Date | Date | Timing |
| Status | Dropdown | Completion |
| Priority | Dropdown | Urgency |
| Notes | Long Text | Context |

### Task Type Options

- Respond to Inquiry
- Send Details
- Send Quote
- Confirm Date
- Collect Deposit
- Send Pre-Visit Info
- Prepare Materials
- Pickup Reminder
- Review Request
- Rebooking Follow-Up
- Class Announcement
- Custom Glass Quote
- General Follow-Up

### Task Status Options

- Not Started
- In Progress
- Waiting
- Completed
- Canceled

---

## 12. Review Request Object / Fields

### Purpose

Tracks review opportunities after successful visits.

### Recommended Fields

| Field | Type | Purpose |
|---|---|---|
| Contact | Linked Contact | Customer |
| Related Event | Linked Event | Visit |
| Review Platform | Dropdown | Where requested |
| Review Request Sent | Checkbox | Status |
| Request Date | Date | Timing |
| Review Completed | Checkbox | Outcome |
| Review Link | URL | Optional |
| Notes | Long Text | Context |

### Review Platform Options

- Google
- Facebook
- TripAdvisor
- Yelp
- Other

---

## 13. Rebooking Opportunity Object

### Purpose

Tracks future repeat business opportunities, especially for groups.

### Example Rebooking Opportunities

- Annual school field trip
- Seasonal homeschool group visit
- Scout troop activity
- Senior group outing
- Corporate team event
- Birthday follow-up
- Holiday workshop
- Future class interest

### Recommended Fields

| Field | Type | Purpose |
|---|---|---|
| Contact | Linked Contact | Organizer |
| Organization | Linked Organization | Group |
| Related Event | Linked Event | Prior visit |
| Opportunity Type | Dropdown | Rebooking category |
| Suggested Follow-Up Date | Date | When to contact |
| Likelihood | Dropdown | Probability |
| Notes | Long Text | Context |
| Status | Dropdown | Stage |

### Opportunity Type Options

- Annual Field Trip
- Seasonal Group Visit
- Birthday Follow-Up
- Corporate Repeat Event
- Class Interest
- Holiday Workshop
- Custom Glass Repeat
- General Repeat Visit

### Opportunity Status Options

- Future Opportunity
- Follow-Up Scheduled
- Contacted
- Interested
- Booked
- Not Interested
- Closed

---

## 14. Custom Glass Request Object

### Purpose

Tracks custom work, repairs, commissions, gifts, and special requests.

### Recommended Fields

| Field | Type | Purpose |
|---|---|---|
| Contact | Linked Contact | Customer |
| Request Type | Dropdown | Kind of custom request |
| Description | Long Text | Request details |
| Reference Photos | File/Link | Optional |
| Desired Size | Text | Scope |
| Color Preferences | Text | Design |
| Deadline | Date | Timing |
| Budget Range | Text/Currency | Fit |
| Feasibility Status | Dropdown | Can it be done? |
| Quote Status | Dropdown | Pricing |
| Quote Amount | Currency | Revenue |
| Deposit Paid | Checkbox | Payment |
| Completion Status | Dropdown | Production |
| Pickup / Shipping Status | Dropdown | Delivery |
| Notes | Long Text | Internal context |

### Request Type Options

- Custom Art
- Repair
- Gift
- Memorial / Sentimental Piece
- Replacement Piece
- Business / Organization Request
- Other

### Feasibility Status Options

- Needs Review
- Feasible
- Maybe
- Not Feasible
- Needs More Information

### Quote Status Options

- Not Quoted
- Quote Needed
- Quote Sent
- Accepted
- Declined
- Revised

### Completion Status Options

- Not Started
- In Progress
- Completed
- Picked Up
- Shipped
- Canceled

---

## 15. Class Interest Record

### Purpose

Tracks people interested in deeper learning, evening classes, weekend classes, one-day classes, two-day classes, or multi-session programs.

### Recommended Fields

| Field | Type | Purpose |
|---|---|---|
| Contact | Linked Contact | Interested person |
| Interest Area | Dropdown/Multi-select | What they want to learn |
| Skill Level | Dropdown | Beginner to advanced |
| Preferred Schedule | Multi-select | Availability |
| Class Format Interest | Multi-select | Format |
| Past Experience | Long Text | Context |
| Signup Date | Date | When joined |
| Announcement Consent | Checkbox | Communication |
| Notes | Long Text | Context |

### Interest Area Options

- Flameworking
- Fused Glass
- Beginner Glass Class
- Torch Skills
- Weekend Workshop
- Evening Class
- Multi-Session Class
- One-Day Class
- Two-Day Class
- Creative Glass Projects
- Not Sure Yet

### Skill Level Options

- Complete Beginner
- Beginner
- Some Experience
- Intermediate
- Advanced
- Unknown

### Preferred Schedule Options

- Weekday Morning
- Weekday Afternoon
- Weekday Evening
- Saturday
- Sunday
- Flexible

### Class Format Options

- One-Day Class
- Two-Day Class
- Multi-Week Class
- Weekend Workshop
- Evening Series
- Private Lesson
- Small Group Class

---

## 16. Source Tracking Model

### Purpose

Tracks where inquiries come from.

This is important for measuring local search, website, AI search, social media, and referral performance.

### Recommended Source Fields

| Field | Type | Purpose |
|---|---|---|
| Inquiry Source | Dropdown | Direct channel |
| Referral Source | Dropdown | Self-reported source |
| Page Source | Dropdown | Website page |
| UTM Source | Text | Future tracking |
| UTM Medium | Text | Future tracking |
| UTM Campaign | Text | Future tracking |
| First Touch Source | Text | Future advanced tracking |
| Last Touch Source | Text | Future advanced tracking |

### Page Source Options

- Home
- Group Tours
- Contact
- Fused Glass Workshops
- Hands-On Glass Experiences
- Field Trips
- Private Events
- Classes
- Custom Glass
- Visit
- FAQ
- Gallery
- Unknown

---

## 17. Priority CRM Views

The CRM should eventually support useful views such as:

### Daily Operations

- New inquiries
- Needs response
- Today’s events
- Upcoming events
- Pickup pending
- Follow-ups due

### Sales / Booking

- Group tour inquiries
- Field trip inquiries
- Private event inquiries
- Quote sent
- Waiting on customer
- Date confirmed

### Customer Growth

- Class interest list
- Rebooking opportunities
- Review requests pending
- Returning customers
- High-value organizations

### Local Search / Marketing

- Inquiries by source
- Inquiries by page
- Inquiries by offer type
- Bookings by source
- Reviews requested vs completed

---

## 18. Minimum Viable CRM Model

For the first CRM version, keep it simple.

Minimum viable fields:

### Contact

- Name
- Email
- Phone
- Customer Type
- Notes

### Inquiry

- Inquiry Type
- Source
- Status
- Preferred Date
- Participant Count
- Age Range
- Message
- Next Follow-Up Date

### Event / Booking

- Event Type
- Event Date
- Participant Count
- Activity Selected
- Payment Status
- Pickup Status
- Review Requested

This is enough to start without overbuilding.

---

## 19. CRM Tool Selection Notes

Do not select CRM software yet.

The CRM field model should be used to evaluate tools later.

A suitable tool should support:

- Custom fields
- Pipeline/status tracking
- Contact records
- Organization records
- Notes
- Tasks
- Form integration
- Email or notification support
- Source tracking
- Export capability
- Automation integration later
- Simple daily use

Possible tool categories later:

- Spreadsheet/Airtable-style database
- Lightweight CRM
- Booking platform with CRM features
- Custom app
- Website form + database
- POS-connected CRM if appropriate

Tool choice should follow workflow clarity.

---

## 20. Automation Readiness

This CRM model prepares future automations such as:

- New inquiry notification
- Auto-reply by inquiry type
- Follow-up reminder
- Quote follow-up
- Deposit reminder
- Pre-visit instruction email
- Pickup reminder
- Review request
- Class announcement
- Rebooking reminder
- Seasonal campaign

Do not build automations until the CRM workflow is confirmed.

---

## 21. Open Questions

Owner input needed later:

- Who will manage CRM daily?
- What tool should be used first?
- Should CRM start as a spreadsheet/Airtable before software?
- Which statuses match the actual workflow best?
- Which fields are too much for daily use?
- What information is currently being lost?
- What follow-ups are currently missed?
- What group inquiries are most valuable?
- How are deposits handled?
- How are pickups currently tracked?
- How are reviews currently requested?
- How should repeat groups be followed up with?
- Should the CRM connect to POS later?
- Should the CRM connect to booking later?
- Should the CRM connect to email marketing later?

---

## 22. Blueprint AI Notes

This document validates Blueprint AI by converting customer journey, offer catalog, group tour strategy, website strategy, listing alignment, and inquiry form design into a practical CRM structure.

The CRM is not just software.

It is the memory and follow-up system for the business.

The CRM should help Payton Glass Center remember the customer, understand the opportunity, follow up properly, and grow repeatable revenue.
