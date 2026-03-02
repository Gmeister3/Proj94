# Personas — Airline Booking System

## Brainstorming & Rough Work

### Step 1 – Identify User Goals

Based on common airline booking system usage patterns, users primarily want to:

- Book flights quickly and confidently
- Find the best price or best itinerary for their trip
- Manage existing bookings (changes, cancellations, seat upgrades)
- Get help when something goes wrong
- Receive clear confirmation and trip details

### Step 2 – Identify User Types (Initial List)

During brainstorming, the following user types were identified:

| Type | Key Traits |
|---|---|
| Frequent business traveler | Books often, values speed, expenses reimbursed |
| Family vacation planner | Multiple passengers, budget-aware, seat preferences |
| Budget / student traveler | Very price-sensitive, flexible dates, infrequent flyer |
| Senior traveler | Less tech-savvy, values clarity, may need accessibility help |
| International / solo traveler | Long-haul, needs visa/passport info, multi-leg itineraries |
| Last-minute traveler | Urgent need, time-sensitive, may pay premium |
| Travel agent / third-party booker | Books on behalf of others, needs group/bulk options |

### Step 3 – Sort & Group

After reviewing the types above, they were grouped by **frequency of use** and **design impact**:

- **High design impact (primary):** Business Traveler, Family Vacation Planner
- **Moderate design impact (secondary):** Budget/Student Traveler, Senior Traveler
- **Edge cases (not represented as full personas):** Travel agent, last-minute traveler

The **Business Traveler** and **Family Vacation Planner** were chosen as primary personas because they represent the largest overlap of features the system must support and have the greatest influence on interface decisions (speed + efficiency vs. multi-passenger guidance + cost clarity). The secondary personas surface important accessibility and affordability requirements without driving the core interaction model.

---

## Primary Personas

---

### Persona 1 – Sarah Chen (Business Traveler)

**Photo placeholder:** *(professional woman, mid-30s)*

| Field | Detail |
|---|---|
| **Name** | Sarah Chen |
| **Age** | 34 |
| **Occupation** | Senior Marketing Manager |
| **Location** | Toronto, ON |
| **Tech Comfort** | High — uses smartphone apps daily, comfortable with web tools |
| **Flight Frequency** | 2–4 times per month (domestic & short-haul international) |
| **Device** | Primarily laptop at work; mobile when travelling |

**Background:**
Sarah travels frequently for client meetings and conferences. Her company has a travel policy that requires booking through approved channels, and all expenses must be submitted afterward. She is always short on time and needs to get in and out of the booking system as fast as possible.

**Goals:**
- Book the correct flight in under 5 minutes
- Find early-morning or late-evening flights to avoid full travel days
- Select aisle seats quickly
- Receive a clear e-ticket and receipt for expense reporting

**Frustrations:**
- Being bombarded with upsells (hotels, car rentals, seat upgrades) mid-booking
- Ambiguous fare rules — does this ticket allow changes?
- Slow or multi-page checkout flows
- Having to re-enter passenger info she has entered before

**Behaviours:**
- Knows exactly what she wants before opening the site
- Uses filters heavily (time of day, number of stops, airline preference)
- Will abandon a booking if the process takes too long or feels untrustworthy
- Reads confirmation emails carefully to ensure details are correct

**Quote:**
> "I just need to get on the right flight. Stop trying to sell me things I didn't ask for."

**Design Implications (Primary):**
- The system **must** support fast, streamlined booking with minimal mandatory steps
- Returning-user profiles to pre-fill passenger details
- Clear fare-type comparison (refundable vs. non-refundable) upfront
- Prominent, uncluttered confirmation page and receipt download

---

### Persona 2 – David Rodriguez (Family Vacation Planner)

**Photo placeholder:** *(man, early 40s, suburban family setting)*

| Field | Detail |
|---|---|
| **Name** | David Rodriguez |
| **Age** | 43 |
| **Occupation** | High School Teacher |
| **Location** | Hamilton, ON |
| **Tech Comfort** | Moderate — comfortable with standard websites; not a power user |
| **Flight Frequency** | 1–2 times per year (family vacation) |
| **Device** | Desktop at home, tablet occasionally |

**Background:**
David books flights for family vacations — typically for himself, his wife, and their two children (ages 8 and 11). He plans carefully, compares prices across several dates, and has a strict budget. He also needs to ensure seats are together, and has questions about baggage for children and stroller policies.

**Goals:**
- Book seats for 4 passengers on the same itinerary with adjacent seating
- Stay within a total budget for the whole family
- Understand baggage policies before completing checkout
- Have a smooth, low-stress experience to look forward to the trip

**Frustrations:**
- Seat maps that don't clearly show which seats are adjacent or available for groups
- Hidden fees that inflate the final price beyond his budget
- Needing to repeat passenger details 4 separate times
- Confusing multi-step checkout where it's unclear how far along he is

**Behaviours:**
- Spends significant time on date-flexibility tools to find the lowest price
- Reads FAQ and baggage policy pages carefully
- Compares at least 2–3 airlines before booking
- Calls customer support if anything is unclear

**Quote:**
> "I just want to know what the actual total cost is before I hand over my credit card."

**Design Implications (Primary):**
- The system **must** surface total price (all fees included) clearly and early
- Multi-passenger data entry should be efficient (copy/duplicate passenger info)
- Seat map must visually indicate available grouped seating
- Progress indicator throughout checkout so users know where they stand

---

## Secondary Personas

---

### Persona 3 – Alex Kim (Budget / Student Traveler)

| Field | Detail |
|---|---|
| **Name** | Alex Kim |
| **Age** | 21 |
| **Occupation** | Undergraduate Student (Computer Science) |
| **Location** | St. Catharines, ON |
| **Tech Comfort** | High — digital native, uses multiple apps and web tools |
| **Flight Frequency** | 1–3 times per year (holidays, visiting family) |
| **Device** | Smartphone primarily |

**Background:**
Alex books flights home for holidays or occasionally for a budget trip with friends. He is extremely price-sensitive and will spend hours finding the cheapest option. He is comfortable with technology but uses it primarily on mobile.

**Goals:**
- Find the absolute lowest price, even if it means inconvenient times or connections
- Understand what's included in a basic fare before purchasing
- Book from a mobile device easily

**Frustrations:**
- Sites that are not mobile-friendly
- Being auto-enrolled in seat selection fees or travel insurance
- Not being able to compare flexible dates easily
- Confusing loyalty program sign-up prompts mid-booking

**Factors Affecting Design (Secondary):**
- Reinforces the need for a **mobile-responsive** interface
- Highlights importance of **opt-in** (not opt-out) add-on services
- Supports the need for a **flexible date search / calendar price view**

---

### Persona 4 – Margaret Thompson (Senior Traveler)

| Field | Detail |
|---|---|
| **Name** | Margaret Thompson |
| **Age** | 68 |
| **Occupation** | Retired Teacher |
| **Location** | Niagara Falls, ON |
| **Tech Comfort** | Low-Moderate — uses email and basic web browsing; struggles with complex layouts |
| **Flight Frequency** | 1–2 times per year (visits grandchildren, leisure travel) |
| **Device** | Desktop computer |

**Background:**
Margaret books flights to visit family and occasionally takes a leisure cruise trip. She is not very comfortable with technology and relies on clear instructions. She sometimes calls airlines directly because she finds websites confusing.

**Goals:**
- Complete a booking without making errors (wrong date, wrong passenger name)
- Understand exactly what she's buying before she confirms
- Be able to request wheelchair assistance or special meals during booking
- Have easy access to customer support if she gets stuck

**Frustrations:**
- Too many options overwhelming the page
- Small text and low-contrast colours
- Inability to easily find the customer support number
- Being forced to create an account before booking

**Factors Affecting Design (Secondary):**
- Reinforces need for **clear, large typography** and high-contrast UI
- Highlights importance of **accessible special services** (wheelchair, meal) during booking
- Supports **guest checkout** option (no forced account creation)
- Underlines the need for **visible, easy-to-find** customer support contact

---

## Summary & Justification

### Primary Personas

| Persona | Why Primary |
|---|---|
| **Sarah Chen** (Business Traveler) | Represents high-frequency users who demand speed and efficiency. Her needs drive the core booking flow — streamlined, fast, and free of unnecessary interruptions. |
| **David Rodriguez** (Family Vacation Planner) | Represents the most complex booking scenario (multiple passengers, seat selection, budget transparency). Designing for him ensures the system works for more casual, detail-oriented users as well. |

Together, these two personas cover the **efficiency** and **completeness** axes of the design space. A system that satisfies both will naturally serve the majority of users.

### Secondary Personas

| Persona | Why Secondary |
|---|---|
| **Alex Kim** (Student/Budget Traveler) | Adds mobile-first and cost-transparency requirements. These refine the design but do not conflict with the primary flow. |
| **Margaret Thompson** (Senior Traveler) | Adds accessibility, simplicity, and support requirements. These enhance usability for all users but are not the primary design driver. |

The secondary personas do not contradict the primary personas — rather, they add constraints that improve the overall experience. Features like mobile responsiveness, accessible typography, and visible customer support benefit all users, not just the secondary ones.

---

*Document prepared for COSC 3P94 — Stage 1, Personas section (Requirements 7 & 8)*
