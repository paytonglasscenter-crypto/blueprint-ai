# Payton Glass Center Inquiry Form Model

Status: Draft
Blueprint AI Phase: Implementation Phase 1.10
Business: Payton Glass Center
Location: Louisville, Kentucky
Depends On: BUSINESS_INTAKE.md, CUSTOMER_JOURNEY.md, OFFER_CATALOG_DETAILED.md, GROUP_TOURS_SYSTEM_DETAILED.md, LOCAL_SEARCH_ALIGNMENT.md, WEBSITE_STRATEGY.md, WEBSITE_PAGE_MAP.md, WEBSITE_CONTENT_BLUEPRINT.md, LOCAL_LISTING_AUDIT.md

---

## 1. Purpose

This document defines the inquiry form model for Payton Glass Center.

The inquiry form is the bridge between:

- Website visitors
- Local search traffic
- AI search traffic
- Group tour inquiries
- Field trip inquiries
- Workshop inquiries
- Private event inquiries
- Class interest
- Custom glass requests
- Future CRM records
- Future automation workflows

The form should not be treated as a generic contact form.

It should collect enough information to help Payton Glass Center respond accurately, reduce back-and-forth, and eventually route inquiries into the right CRM and automation paths.

---

## 2. Core Principle

The form should be simple for customers but structured enough for the business.

A weak form only asks:

- Name
- Email
- Message

A stronger form helps identify:

- Who the customer is
- What they want
- Which offer they are interested in
- Whether they are an individual, group, school, or organization
- How many people are involved
- What date or timeframe they want
- What follow-up path should happen next

The goal is not to overcomplicate the form.

The goal is to ask the right questions at the right time.

---

## 3. Primary Form Goal

The primary goal of the inquiry form is to capture high-quality inquiries for:

1. Group Tours
2. Field Trips
3. Fused Glass Workshops
4. Hands-On Torch Experiences
5. Private Events
6. Birthday Activities
7. Class Interest
8. Custom Glass
9. Glass Art / Gifts
10. General Questions

The form should support all major inquiry types while allowing future filtering, tagging, CRM routing, and automation.

---

## 4. Recommended Main Inquiry Form

### Form Name

Request a Tour, Workshop, Event, or Glass Inquiry

### Recommended Page

`/contact`

or

`/request-a-booking`

### Primary CTA

Send Request

### Intro Copy Draft

Use the form below to ask about group tours, fused glass workshops, hands-on glass experiences, field trips, private events, classes, custom glass, gifts, or general questions.

For group requests, please include as many details as possible so the studio can respond accurately.

---

## 5. Core Fields

These fields should appear on the main form.

### Contact Information

- Name
- Email
- Phone

### Inquiry Type

- Offer interest
- Message

### Scheduling Information

- Preferred date
- Preferred time
- Backup date
- Flexible dates? yes/no

### Group Information

- Group type
- Organization name
- Number of participants
- Number of non-participating guests or chaperones
- Age range or grade level

### Context Information

- How did you hear about us?
- Special needs, accessibility notes, or important details
- Permission to text? yes/no if legally appropriate later

---

## 6. Recommended Required Fields

The first version should require only the fields needed to respond.

Recommended required fields:

- Name
- Email or phone
- Offer interest
- Message

Recommended optional but encouraged fields:

- Phone
- Preferred date
- Preferred time
- Group type
- Organization name
- Number of participants
- Age range
- How did you hear about us?

This keeps the form from becoming too heavy while still collecting useful details.

---

## 7. Offer Interest Options

Recommended offer interest dropdown:

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

### Notes

These labels should match the website, local listings, CRM, and future automations.

Do not use too many confusing variations of the same offer.

---

## 8. Group Type Options

Recommended group type dropdown:

- Family
- School
- Homeschool Group
- Scout / Youth Group
- Senior Group
- Corporate Team
- Church Group
- Tourist Group
- Birthday Group
- Friend Group
- Club / Organization
- Community Group
- Individual / Couple
- Other

### Notes

Group type helps route the inquiry and understand customer intent.

It also becomes useful later for CRM segmentation, follow-up, rebooking reminders, and marketing analysis.

---

## 9. Referral Source Options

Recommended “How did you hear about us?” options:

- Google Search
- Google Maps
- Google Business Profile
- Bing Search
- Apple Maps
- AI Search / ChatGPT / Perplexity / Gemini
- Facebook
- Instagram
- YouTube
- TikTok
- Friend / Word of Mouth
- School / Organization Referral
- Louisville Tourism / Local Directory
- Returning Customer
- Drove By / Saw Sign
- Other

### Notes

This field will eventually help measure which visibility channels produce real inquiries.

It also supports Blueprint AI’s local search and AI search validation.

---

## 10. Main Form Field Model

| Field | Type | Required? | Purpose | Future CRM Field |
|---|---|---:|---|---|
| Name | Text | Yes | Identify contact | Contact Name |
| Email | Email | Conditional | Contact method | Email |
| Phone | Phone | Conditional | Contact method | Phone |
| Preferred Contact Method | Dropdown | No | Helps response method | Preferred Contact Method |
| Offer Interest | Dropdown | Yes | Routes inquiry | Inquiry Type |
| Message | Long Text | Yes | Captures request | Inquiry Notes |
| Preferred Date | Date | No | Scheduling | Preferred Date |
| Preferred Time | Text/Dropdown | No | Scheduling | Preferred Time |
| Backup Date | Date | No | Scheduling flexibility | Backup Date |
| Flexible Dates | Yes/No | No | Scheduling flexibility | Flexible Dates |
| Group Type | Dropdown | No | Segment | Group Type |
| Organization Name | Text | No | School/company/group | Organization |
| Participant Count | Number | No | Capacity planning | Participant Count |
| Non-Participant Count | Number | No | Chaperones/guests | Non-Participant Count |
| Age Range / Grade Level | Text | No | Suitability | Age Range |
| Special Notes | Long Text | No | Accessibility/details | Special Notes |
| Referral Source | Dropdown | No | Marketing source | Referral Source |
| Consent to Text | Checkbox | Later | SMS compliance | SMS Consent |

### Conditional Contact Rule

At least one contact method should be required:

- Email
- Phone

The form should not require both unless necessary.

---

## 11. Group Tour Inquiry Fields

When the offer interest is Group Tour, the form should encourage:

- Group type
- Organization name
- Number of participants
- Age range
- Preferred date
- Preferred time
- Backup date
- Desired activity
- Special needs or accessibility notes
- Whether this is a school, senior, corporate, church, tourist, or private group

### Group Tour Prompt Copy

Tell us about your group, preferred date, group size, age range, and what kind of glass activity you are interested in.

### Future Routing

Group Tour inquiries should eventually route to:

- Group tour CRM pipeline
- Group inquiry response template
- Scheduling follow-up
- Pre-visit instruction workflow
- Review and rebooking workflow

---

## 12. Field Trip Inquiry Fields

When the offer interest is Field Trip, the form should encourage:

- School or organization name
- Grade level
- Number of students
- Number of chaperones
- Preferred date
- Preferred time
- Educational goals
- Activity interest
- Accessibility or special needs
- Teacher/coordinator contact information

### Field Trip Prompt Copy

Tell us your school or organization name, student count, grade level, preferred date, and what kind of educational visit you are planning.

### Future Routing

Field Trip inquiries should eventually route to:

- Field trip CRM pipeline
- Teacher/group organizer response
- Educational visit planning template
- Annual rebooking reminder

---

## 13. Fused Glass Workshop Inquiry Fields

When the offer interest is Fused Glass Workshop, the form should encourage:

- Number of participants
- Age range
- Preferred date
- Preferred time
- Project interest if known
- Group or individual participation
- Pickup questions if relevant

### Fused Glass Prompt Copy

Tell us how many people would like to participate, the age range, preferred date, and whether you are asking for an individual visit, family activity, or group workshop.

### Future Routing

Fused Glass inquiries should eventually route to:

- Workshop inquiry pipeline
- Workshop confirmation template
- Pickup reminder workflow
- Review request workflow

---

## 14. Hands-On Torch Experience Inquiry Fields

When the offer interest is Hands-On Torch Experience, the form should encourage:

- Number of participants
- Age range
- Preferred date
- Preferred time
- Experience level
- Whether it is for an individual, couple, family, or small group
- Project interest if known

### Hands-On Torch Prompt Copy

Tell us how many people are interested, your preferred date, age range, and whether you are looking for an individual, couple, family, or small group experience.

### Future Routing

Hands-On Torch inquiries should eventually route to:

- Hands-on experience inquiry pipeline
- Safety/preparation message
- Scheduling follow-up
- Pickup reminder if needed
- Future class invitation

---

## 15. Private Event Inquiry Fields

When the offer interest is Private Event or Birthday Activity, the form should encourage:

- Event type
- Group size
- Age range
- Preferred date
- Preferred time
- Activity interest
- Food/drink questions
- Special requests
- Budget expectations if useful later

### Private Event Prompt Copy

Tell us what type of event you are planning, how many people may attend, the age range, preferred date, and what kind of activity you are interested in.

### Future Routing

Private Event inquiries should eventually route to:

- Private event CRM pipeline
- Event planning response
- Deposit reminder if applicable
- Pre-event information
- Review request
- Birthday anniversary follow-up if appropriate

---

## 16. Class Interest Fields

When the offer interest is Class Interest, the form should encourage:

- Skill level
- Interest area
- Preferred schedule
- Evening/weekend availability
- One-day, multi-day, or multi-session interest
- Past experience
- Email signup consent if appropriate

### Class Interest Prompt Copy

Tell us what kind of glass class you are interested in, your skill level, and whether evenings, weekends, one-day classes, or multi-session classes work best for you.

### Future Routing

Class Interest inquiries should eventually route to:

- Class interest list
- Future class announcement workflow
- Segment by skill level
- Segment by schedule preference
- Next-level class invitation

---

## 17. Custom Glass Inquiry Fields

When the offer interest is Custom Glass, the form should encourage:

- Project description
- Desired size
- Color preferences
- Deadline
- Budget range if appropriate
- Whether the customer has photos or references
- Whether repair is requested
- Pickup or shipping needs

### Custom Glass Prompt Copy

Describe what you are looking for, including size, colors, timeline, repair needs, or reference photos if available.

### Future Routing

Custom Glass inquiries should eventually route to:

- Custom glass quote process
- Feasibility review
- Quote follow-up
- Deposit/payment workflow if applicable
- Completion and pickup/shipping workflow

---

## 18. Glass Art / Gift Inquiry Fields

When the offer interest is Glass Art / Gift, the form should encourage:

- Gift occasion
- Product type
- Price range if appropriate
- Pickup or shipping need
- Timeline
- Customization interest

### Gift Inquiry Prompt Copy

Tell us what kind of handmade glass gift or item you are looking for, your timeline, and whether you need pickup, shipping, or custom options.

### Future Routing

Glass Art / Gift inquiries should eventually route to:

- Retail/gift inquiry
- Seasonal offer follow-up
- Custom glass upsell if appropriate
- Gift reminder campaign if appropriate

---

## 19. Form Confirmation Message

After form submission, customers should see a clear confirmation.

### Draft Confirmation Message

Thank you for contacting Payton Glass Center.

Your request has been received. The studio will review your details and follow up about availability, options, pricing, and next steps.

For group requests, the more details you provide, the easier it is for us to respond accurately.

### Future Improvement

Later, the confirmation message can vary by inquiry type.

Examples:

- Group Tour confirmation
- Field Trip confirmation
- Workshop confirmation
- Custom Glass confirmation
- Class Interest confirmation

---

## 20. Auto-Reply Email Draft Structure

Future auto-replies should be offer-specific.

The first basic auto-reply can include:

- Thank you
- Confirmation that the request was received
- Summary of submitted details if possible
- Expected response timeframe
- Reminder to provide missing group details
- Link to FAQ or relevant page
- Contact information

Automation should not be built yet.

This document only defines the model.

---

## 21. Spam and Quality Controls

The form should include basic protections:

- Spam protection
- Required contact method
- Honeypot field if available
- Clear labels
- Avoid overly long required fields
- Avoid asking for sensitive unnecessary information
- Validate email format
- Validate phone format if possible
- Store submission date/time
- Store page source later if possible

---

## 22. Accessibility and Usability Requirements

The form should be:

- Mobile-friendly
- Easy to read
- Clear on required fields
- Keyboard accessible
- Screen-reader friendly
- Not too long on first load
- Broken into logical sections if needed
- Clear after submission
- Error messages should be understandable

---

## 23. Data Privacy Notes

The inquiry form should only collect information needed to respond to the customer.

Do not collect unnecessary sensitive information.

If SMS/text consent is added later, it should be handled carefully and clearly.

If newsletter or class announcement signup is added later, consent should be explicit.

---

## 24. CRM Mapping

This inquiry form should eventually feed CRM records.

Recommended CRM objects or record types:

- Contact
- Organization
- Inquiry
- Event / Booking
- Offer Interest
- Follow-Up Task
- Pickup Task if needed
- Review Request if completed
- Rebooking Opportunity if applicable

Recommended first-stage CRM statuses:

- New Inquiry
- Needs Response
- Waiting on Customer
- Quote / Details Sent
- Date Requested
- Date Confirmed
- Confirmed
- Completed
- Pickup Pending
- Review Requested
- Rebooking Opportunity
- Closed Lost
- Canceled

---

## 25. Automation Mapping

Future automation triggers may include:

### On Form Submission

- Send internal notification
- Create CRM record
- Tag inquiry type
- Send customer confirmation

### If Group Tour

- Send group tour response
- Create scheduling task
- Create pre-visit task if confirmed

### If Field Trip

- Send educational visit response
- Create school follow-up task
- Create annual rebooking reminder later

### If Class Interest

- Add to class interest list
- Tag by preferred schedule and skill level

### If Custom Glass

- Create custom quote task
- Request photos if missing

Automation should wait until the CRM field model is complete.

---

## 26. Website Page Placement

The inquiry form should appear on:

- Contact / Request a Booking page

Shorter inquiry CTAs should appear on:

- Home
- Group Tours
- Fused Glass Workshops
- Hands-On Glass Experiences
- Field Trips
- Private Events
- Classes
- Custom Glass
- Visit
- FAQ

Each CTA should lead to the form, ideally with offer interest preselected later.

---

## 27. Tracking Requirements Later

Future tracking should identify:

- Page where inquiry started
- Offer interest
- Referral source
- Device type if available
- Local search source if known
- AI search source if self-reported
- Conversion page
- Date/time
- Response time
- Booking outcome
- Revenue outcome later if appropriate

This will help Blueprint AI validate which website and listing surfaces generate real business value.

---

## 28. Open Questions

Owner input needed later:

- Should phone or email be preferred?
- Should both phone and email be required?
- What is the preferred response timeframe?
- Should text messaging be used?
- What booking tool, if any, will be connected later?
- Should prices be shown before the form?
- Should group tours have a separate form?
- Should custom glass have a separate form?
- Should class interest have a separate form?
- Should the form support file uploads for custom glass photos?
- Which fields are too much for first launch?
- Which inquiries are highest priority?
- Who receives form submissions?
- Where should submissions be stored before CRM?

---

## 29. First Version Recommendation

For the first website version, use one main structured inquiry form.

Keep it simple but useful.

Recommended first version:

Required:

- Name
- Email or phone
- Offer interest
- Message

Optional:

- Phone
- Preferred date
- Preferred time
- Group type
- Organization name
- Number of participants
- Age range
- Backup date
- How did you hear about us?
- Special notes

Later, add conditional logic by offer type if the website platform supports it.

---

## 30. Blueprint AI Notes

This document validates Blueprint AI by turning the website strategy into a structured inquiry intake system.

The inquiry form becomes the first operational bridge between:

- Website
- Local search
- AI search
- Customer journey
- Offer catalog
- CRM
- Automation
- Follow-up
- Revenue tracking

The form should serve real business operations, not just collect messages.
