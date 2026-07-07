# Payton Glass Center Inquiry Form Build Spec

Status: Draft
Blueprint AI Phase: Implementation Phase 3.5
Business: Payton Glass Center
Location: Louisville, Kentucky
Phase Focus: First inquiry form build specification
Depends On: INQUIRY_FORM_MODEL.md, CRM_FIELD_MODEL.md, AUTOMATION_TRIGGER_MODEL.md, WEBSITE_BUILD_PLAN.md

---

## 1. Purpose

This document defines the first inquiry form build specification for Payton Glass Center.

The first website should not launch with a vague contact form.

It should use a structured inquiry form that helps customers provide useful details and helps the business respond efficiently.

This form should support:

- Group tour inquiries
- Field trip inquiries
- Fused glass workshop inquiries
- Hands-on glass experience inquiries
- Private event inquiries
- Birthday activity inquiries
- Class interest inquiries
- Custom glass inquiries
- General questions

The form should remain simple enough to launch quickly while being structured enough for future CRM and automation.

---

## 2. Core Principle

Capture useful inquiry information without overcomplicating the customer experience.

The first form should not try to finalize bookings, collect deposits, confirm dates, quote prices, or automate approval.

It should collect enough information for Payton Glass Center to respond intelligently.

---

## 3. First Form Name

Recommended public name:

**Request a Tour, Workshop, Event, or Glass Inquiry**

Shorter possible name:

**Request Information**

Button label:

**Send Request**

---

## 4. Primary Form Location

The form should appear on:

- `/contact/`

The form should also be linked from:

- Home
- Group Tours
- Fused Glass Workshops
- Hands-On Glass Experiences
- Field Trips
- Private Events
- FAQ
- Visit
- Gallery / Glass Art
- Classes if included later
- Custom Glass if included later

### CTA Language Examples

- Request a Group Tour
- Ask About Availability
- Plan a Field Trip
- Request a Private Event
- Ask About Fused Glass
- Ask About Hands-On Glass Experiences
- Contact the Studio
- Join the Class Interest List

---

## 5. First Form Goals

The form should help answer:

- Who is contacting the studio?
- How should the studio respond?
- What are they interested in?
- Is this an individual, family, school, organization, or group?
- How many people are involved?
- What age range is involved?
- What date/time are they hoping for?
- What details or questions do they have?
- How did they hear about Payton Glass Center?
- Does this inquiry need special handling?

---

## 6. Required Fields

The first form should require only the most essential information.

| Field | Type | Required? | Notes |
|---|---|---:|---|
| Name | Text | Yes | Contact person |
| Email | Email | Yes | Primary response method |
| Phone | Phone | Yes | Useful for group/event follow-up |
| Offer Interest | Dropdown | Yes | Main routing field |
| Message | Long text | Yes | Lets customer explain |

### Required Field Principle

Do not require too many fields.

A group organizer should be encouraged to give details, but the form should not become so long that people abandon it.

---

## 7. Recommended Optional Fields

| Field | Type | Required? | Notes |
|---|---|---:|---|
| Group Type | Dropdown | No | Useful for tours, field trips, events |
| Organization Name | Text | No | School, company, church, etc. |
| Number of Participants | Number | No | Needed for capacity planning |
| Number of Observers / Chaperones | Number | No | Useful for field trips/groups |
| Age Range / Grade Level | Text | No | Important for safety and activity choice |
| Preferred Date | Date | No | Helps scheduling |
| Preferred Time | Text or time | No | Allows flexible entry |
| Backup Date | Date | No | Useful for groups |
| How Did You Hear About Us? | Dropdown | No | Source tracking |
| Special Notes | Long text | No | Accessibility, timing, questions |

---

## 8. Offer Interest Dropdown

Recommended options:

1. Group Tour
2. Field Trip
3. Fused Glass Workshop
4. Hands-On Torch Experience
5. Private Event
6. Birthday Activity
7. Class Interest
8. Custom Glass
9. Glass Art / Gift
10. Demonstration / Studio Visit
11. General Question

### Notes

Offer names should match the website and CRM model.

Do not use too many similar choices.

If customers are likely to be confused, the form can include a helper line:

**Not sure which option to choose? Select “General Question” and tell us what you are looking for.**

---

## 9. Group Type Dropdown

Recommended options:

1. School
2. Homeschool Group
3. Scout / Youth Group
4. Senior Group
5. Corporate / Team
6. Church / Community Group
7. Birthday Group
8. Family / Friends
9. Tourist Group
10. Club / Organization
11. Individual / Couple
12. Other
13. Not Applicable

---

## 10. Referral Source Dropdown

Recommended options:

1. Google Search
2. Google Maps
3. Google Business Profile
4. Bing
5. Apple Maps
6. Facebook
7. Instagram
8. YouTube
9. Friend / Word of Mouth
10. School / Organization
11. Returning Customer
12. Drove By / Saw the Studio
13. Event / Tourism Listing
14. Other

---

## 11. Conditional Field Logic

The first form can launch without conditional logic.

However, future versions may show different fields based on Offer Interest.

### If Group Tour

Encourage:

- Group type
- Organization name
- Participant count
- Age range
- Preferred date/time
- Backup date

### If Field Trip

Encourage:

- School/organization name
- Grade level
- Number of students
- Number of chaperones
- Preferred date/time
- Educational goals

### If Fused Glass Workshop

Encourage:

- Number of participants
- Age range
- Preferred date/time
- Project interest

### If Hands-On Torch Experience

Encourage:

- Number of participants
- Age range
- Preferred date/time
- Experience level

### If Private Event / Birthday Activity

Encourage:

- Event type
- Participant count
- Age range
- Preferred date/time
- Food/drink questions
- Activity interest

### If Class Interest

Encourage:

- Skill level
- Preferred schedule
- Evening/weekend availability
- Type of class desired

### If Custom Glass

Encourage:

- Project description
- Deadline
- Budget range if appropriate
- Reference photo upload later
- Pickup/shipping need

---

## 12. Initial Form Version Recommendation

First launch version should use a single simple form.

### Version 1 Fields

Required:

- Name
- Email
- Phone
- Offer Interest
- Message

Optional:

- Group Type
- Organization Name
- Number of Participants
- Age Range / Grade Level
- Preferred Date
- Preferred Time
- Backup Date
- How Did You Hear About Us?
- Special Notes

### Do Not Include Yet

- Payment
- Deposit collection
- Exact scheduling calendar
- Automatic booking confirmation
- File upload unless custom glass workflow is ready
- Waiver system
- Account creation
- Customer login
- AI chat response
- Automatic quote

---

## 13. Customer Confirmation Message

After form submission, show this message:

```text
Thank you for contacting Payton Glass Center.

Your request has been received. We will review your details and follow up about availability, options, pricing, and next steps.

For group tours, field trips, private events, and hands-on experiences, the more details you provide, the easier it is for us to respond accurately.
