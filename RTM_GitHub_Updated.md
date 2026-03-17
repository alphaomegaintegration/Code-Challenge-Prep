# C2C Hub – Requirements Traceability Matrix (RTM)

**Solicitation:** 70SBUR26Q00000001  
**Challenge:** ODOS 3.1 DevSecOps & UXD/IxD Coding Challenge  
**Sprint:** 7-Day DevSecOps Delivery Sprint

## Coverage Dashboard

| Metric | Count |
|---|---|
| Personas | 3 |
| Epics | 7 |
| User Stories / RTM Entries | 46 |

## Navigation

Jump to: [Administrator](#persona-administrator) • [Shuttle Operator](#persona-shuttle-operator) • [Student](#persona-student) • [Epic View](#epic-view)

---

## RTM by Persona

### Persona: Administrator
<a id='persona-administrator'></a>

| RTM-ID   | Story ID   | Epic                             | User Story Title                             | Priority (MoSCoW)   | MVP Scope?   |
|:---------|:-----------|:---------------------------------|:---------------------------------------------|:--------------------|:-------------|
| RTM-024  | O31-31     | Epic 6 – Admin Operations Center | Manage Student Registrations                 | Must                | Yes          |
| RTM-025  | O31-32     | Epic 6 – Admin Operations Center | View, Edit, Cancel Bookings & Seat Overrides | Must                | Yes          |
|          | O31-13     |                                  |                                              |                     |              |
| RTM-026  | O31-33     | Epic 6 – Admin Operations Center | Manage Shuttle Stops with Notifications      | Must                | Yes          |
| RTM-027  | O31-34     | Epic 6 – Admin Operations Center | Manage Shuttle Driver Profiles               | Must                | Yes          |
| RTM-028  | O31-35     | Epic 6 – Admin Operations Center | View Performance Ratings                     | Must                | Yes          |
| RTM-029  | O31-50     | Epic 6 – Admin Operations Center | Demand Forecasting Dashboard                 | Must                | Yes          |
| RTM-030  | O31-53     | Epic 6 – Admin Operations Center | Strategic Pricing Engine                     | Should              | No           |
| RTM-031  | O31-54     | Epic 6 – Admin Operations Center | Incident Command Push Notifications          | Should              | No           |
| RTM-032  | O31-55     | Epic 6 – Admin Operations Center | Geofencing Route Monitoring                  | Should              | No           |
| RTM-033  | O31-51     | Epic 6 – Admin Operations Center | Sales & Occupancy Analytics                  | Must                | Yes          |
| RTM-034  | O31-56     | Epic 6 – Admin Operations Center | Automated Billing Reports Viewer             | Should              | No           |
| RTM-035  | O31-57     | Epic 6 – Admin Operations Center | Process Rescheduling / Cancellation Credits  | Should              | No           |
| RTM-036  | O31-58     | Epic 6 – Admin Operations Center | Review & Respond to Student Comments         | Should              | No           |
| RTM-037  | O31-59     | Epic 6 – Admin Operations Center | Mass Promotional Notifications               | Should              | No           |
| RTM-038  | O31-52     | Epic 6 – Admin Operations Center | SES / SNS Notification Dashboard             | Should              | No           |
| RTM-039  | O31-60     | Epic 6 – Admin Operations Center | Fleet Health & Scheduled Maintenance         | Could               | No           |
| RTM-040  | O31-61     | Epic 6 – Admin Operations Center | Shuttle Video Recording Viewer               | Could               | No           |
| RTM-043  | O31-62     | Epic 6 – Admin Operations Center | Respond to Performance Ratings               | Should              | No           |
| RTM-048  | O31-83     | Epic 6 – Admin Operations Center | Manage Shuttle Path Dashboard                | Must                | Yes          |


### Persona: Shuttle Operator
<a id='persona-shuttle-operator'></a>

| RTM-ID   | Story ID   | Epic                            | User Story Title                     | Priority (MoSCoW)   | MVP Scope?   |
|:---------|:-----------|:--------------------------------|:-------------------------------------|:--------------------|:-------------|
| RTM-041  | "O31-38    | Epic 7 – Shuttle Operator Tools | Real-Time Digital Passenger Manifest | Must                | Yes          |
|          |            |                                 |                                      |                     |              |
|          | O31-14"    |                                 |                                      |                     |              |


### Persona: Student
<a id='persona-student'></a>

| RTM-ID   | Story ID   | Epic                                               | User Story Title                                      | Priority (MoSCoW)   | MVP Scope?   |
|:---------|:-----------|:---------------------------------------------------|:------------------------------------------------------|:--------------------|:-------------|
| RTM-001  | "O31-7     | Epic 1 – Student Onboarding                        | Student Registration with Profile Details             | Must                | Yes          |
|          |            |                                                    |                                                       |                     |              |
|          | O31-36"    |                                                    |                                                       |                     |              |
| RTM-002  | O31-37     | Epic 1 – Student Onboarding                        | Secure Login & Session Management                     | Must                | Yes          |
| RTM-003  | O31-39     | Epic 1 – Student Onboarding                        | Subsidized Equity Credits (Financial Aid Wallet)      | Should              | No           |
| RTM-004  | O31-40     | Epic 1 – Student Onboarding                        | Exam Schedule Integration Sync                        | Could               | No           |
| RTM-005  | O31-9      | Epic 2 – Integrated Search & Safe Transfer Booking | Unified Flight & Shuttle Search with Date Flexibility | Must                | Yes          |
| RTM-006  | O31-10     | Epic 2 – Integrated Search & Safe Transfer Booking | Shuttle Stop / Pickup Selection                       | Must                | Yes          |
| RTM-007  | O31-24     | Epic 2 – Integrated Search & Safe Transfer Booking | Safe Transfer Window Filtering                        | Must                | Yes          |
| RTM-008  | O31-25     | Epic 2 – Integrated Search & Safe Transfer Booking | Booking Confirmation with Payment                     | Must                | Yes          |
| RTM-010  | O31-70     | Epic 2 – Integrated Search & Safe Transfer Booking | Early Bird Deal Recommendations                       | Should              | No           |
| RTM-011  | O31-12     | Epic 3 – Digital Boarding & Real-Time Tracking     | Digital Boarding Pass / QR Code                       | Must                | Yes          |
| RTM-012  | O31-26     | Epic 3 – Digital Boarding & Real-Time Tracking     | Real-Time GPS Shuttle Tracking                        | Must                | Yes          |
| RTM-013  | O31-12     | Epic 3 – Digital Boarding & Real-Time Tracking     | Apple / Google Wallet Integration                     | Should              | No           |
| RTM-014  | O31-27     | Epic 4 – Booking Lifecycle & Notifications         | Email Booking Notifications                           | Must                | Yes          |
| RTM-015  | O31-28     | Epic 4 – Booking Lifecycle & Notifications         | Cancellation with Credit to Wallet                    | Must                | Yes          |
| RTM-016  | O31-44     | Epic 4 – Booking Lifecycle & Notifications         | Flight Delay Rescheduling Automation                  | Must                | Yes          |
| RTM-017  | O31-45     | Epic 4 – Booking Lifecycle & Notifications         | Emergency Shuttle Breakdown Notifications             | Must                | Yes          |
| RTM-018  | O31-46     | Epic 4 – Booking Lifecycle & Notifications         | Exam Schedule Booking Reminders & Deal Alerts         | Could               | No           |
| RTM-019  | O31-29     | Epic 5 – Student Engagement & Social Features      | Performance Ratings & Comments                        | Must                | Yes          |
| RTM-020  | O31-30     | Epic 5 – Student Engagement & Social Features      | Tips / Gratuity for Shuttle Drivers                   | Must                | Yes          |
| RTM-021  | "O31-47    | Epic 5 – Student Engagement & Social Features      | Ride-Share Buddy Matching                             | Should              | No           |
|          |            |                                                    |                                                       |                     |              |
|          | O31-33"    |                                                    |                                                       |                     |              |
| RTM-022  | O31-48     | Epic 5 – Student Engagement & Social Features      | Study-on-the-Go Group Booking                         | Could               | No           |
| RTM-023  | O31-49     | Epic 5 – Student Engagement & Social Features      | Last-Seat Emergency Protocol                          | Could               | No           |
| RTM-042  | O31-79     | Epic 4 – Booking Lifecycle & Notifications         | Text/SMS Booking Notifications                        | Should              | No           |
| RTM-044  | O31-63     | Epic 1 – Student Onboarding                        | Student Dashboard                                     | Must                | Yes          |
| RTM-045  | O31-70     | Epic 1 – Student Onboarding                        | Upcoming Trips Section                                | Must                | Yes          |
| RTM-047  | O31-72     | Epic 2 – Integrated Search & Safe Transfer Booking | Search Results Page                                   | Must                | Yes          |



---

## Epic View
<a id='epic-view'></a>

### Epic 1 – Student Onboarding

| RTM-ID   | Story ID   | Persona   | User Story Title                                 | Priority (MoSCoW)   | MVP Scope?   |
|:---------|:-----------|:----------|:-------------------------------------------------|:--------------------|:-------------|
| RTM-001  | "O31-7     | Student   | Student Registration with Profile Details        | Must                | Yes          |
|          |            |           |                                                  |                     |              |
|          | O31-36"    |           |                                                  |                     |              |
| RTM-002  | O31-37     | Student   | Secure Login & Session Management                | Must                | Yes          |
| RTM-003  | O31-39     | Student   | Subsidized Equity Credits (Financial Aid Wallet) | Should              | No           |
| RTM-004  | O31-40     | Student   | Exam Schedule Integration Sync                   | Could               | No           |
| RTM-044  | O31-63     | Student   | Student Dashboard                                | Must                | Yes          |
| RTM-045  | O31-70     | Student   | Upcoming Trips Section                           | Must                | Yes          |


### Epic 2 – Integrated Search & Safe Transfer Booking

| RTM-ID   | Story ID   | Persona   | User Story Title                                      | Priority (MoSCoW)   | MVP Scope?   |
|:---------|:-----------|:----------|:------------------------------------------------------|:--------------------|:-------------|
| RTM-005  | O31-9      | Student   | Unified Flight & Shuttle Search with Date Flexibility | Must                | Yes          |
| RTM-006  | O31-10     | Student   | Shuttle Stop / Pickup Selection                       | Must                | Yes          |
| RTM-007  | O31-24     | Student   | Safe Transfer Window Filtering                        | Must                | Yes          |
| RTM-008  | O31-25     | Student   | Booking Confirmation with Payment                     | Must                | Yes          |
| RTM-010  | O31-70     | Student   | Early Bird Deal Recommendations                       | Should              | No           |
| RTM-047  | O31-72     | Student   | Search Results Page                                   | Must                | Yes          |


### Epic 3 – Digital Boarding & Real-Time Tracking

| RTM-ID   | Story ID   | Persona   | User Story Title                  | Priority (MoSCoW)   | MVP Scope?   |
|:---------|:-----------|:----------|:----------------------------------|:--------------------|:-------------|
| RTM-011  | O31-12     | Student   | Digital Boarding Pass / QR Code   | Must                | Yes          |
| RTM-012  | O31-26     | Student   | Real-Time GPS Shuttle Tracking    | Must                | Yes          |
| RTM-013  | O31-12     | Student   | Apple / Google Wallet Integration | Should              | No           |


### Epic 4 – Booking Lifecycle & Notifications

| RTM-ID   | Story ID   | Persona   | User Story Title                              | Priority (MoSCoW)   | MVP Scope?   |
|:---------|:-----------|:----------|:----------------------------------------------|:--------------------|:-------------|
| RTM-014  | O31-27     | Student   | Email Booking Notifications                   | Must                | Yes          |
| RTM-015  | O31-28     | Student   | Cancellation with Credit to Wallet            | Must                | Yes          |
| RTM-016  | O31-44     | Student   | Flight Delay Rescheduling Automation          | Must                | Yes          |
| RTM-017  | O31-45     | Student   | Emergency Shuttle Breakdown Notifications     | Must                | Yes          |
| RTM-018  | O31-46     | Student   | Exam Schedule Booking Reminders & Deal Alerts | Could               | No           |
| RTM-042  | O31-79     | Student   | Text/SMS Booking Notifications                | Should              | No           |


### Epic 5 – Student Engagement & Social Features

| RTM-ID   | Story ID   | Persona   | User Story Title                    | Priority (MoSCoW)   | MVP Scope?   |
|:---------|:-----------|:----------|:------------------------------------|:--------------------|:-------------|
| RTM-019  | O31-29     | Student   | Performance Ratings & Comments      | Must                | Yes          |
| RTM-020  | O31-30     | Student   | Tips / Gratuity for Shuttle Drivers | Must                | Yes          |
| RTM-021  | "O31-47    | Student   | Ride-Share Buddy Matching           | Should              | No           |
|          |            |           |                                     |                     |              |
|          | O31-33"    |           |                                     |                     |              |
| RTM-022  | O31-48     | Student   | Study-on-the-Go Group Booking       | Could               | No           |
| RTM-023  | O31-49     | Student   | Last-Seat Emergency Protocol        | Could               | No           |


### Epic 6 – Admin Operations Center

| RTM-ID   | Story ID   | Persona       | User Story Title                             | Priority (MoSCoW)   | MVP Scope?   |
|:---------|:-----------|:--------------|:---------------------------------------------|:--------------------|:-------------|
| RTM-024  | O31-31     | Administrator | Manage Student Registrations                 | Must                | Yes          |
| RTM-025  | O31-32     | Administrator | View, Edit, Cancel Bookings & Seat Overrides | Must                | Yes          |
|          | O31-13     |               |                                              |                     |              |
| RTM-026  | O31-33     | Administrator | Manage Shuttle Stops with Notifications      | Must                | Yes          |
| RTM-027  | O31-34     | Administrator | Manage Shuttle Driver Profiles               | Must                | Yes          |
| RTM-028  | O31-35     | Administrator | View Performance Ratings                     | Must                | Yes          |
| RTM-029  | O31-50     | Administrator | Demand Forecasting Dashboard                 | Must                | Yes          |
| RTM-030  | O31-53     | Administrator | Strategic Pricing Engine                     | Should              | No           |
| RTM-031  | O31-54     | Administrator | Incident Command Push Notifications          | Should              | No           |
| RTM-032  | O31-55     | Administrator | Geofencing Route Monitoring                  | Should              | No           |
| RTM-033  | O31-51     | Administrator | Sales & Occupancy Analytics                  | Must                | Yes          |
| RTM-034  | O31-56     | Administrator | Automated Billing Reports Viewer             | Should              | No           |
| RTM-035  | O31-57     | Administrator | Process Rescheduling / Cancellation Credits  | Should              | No           |
| RTM-036  | O31-58     | Administrator | Review & Respond to Student Comments         | Should              | No           |
| RTM-037  | O31-59     | Administrator | Mass Promotional Notifications               | Should              | No           |
| RTM-038  | O31-52     | Administrator | SES / SNS Notification Dashboard             | Should              | No           |
| RTM-039  | O31-60     | Administrator | Fleet Health & Scheduled Maintenance         | Could               | No           |
| RTM-040  | O31-61     | Administrator | Shuttle Video Recording Viewer               | Could               | No           |
| RTM-043  | O31-62     | Administrator | Respond to Performance Ratings               | Should              | No           |
| RTM-048  | O31-83     | Administrator | Manage Shuttle Path Dashboard                | Must                | Yes          |


### Epic 7 – Shuttle Operator Tools

| RTM-ID   | Story ID   | Persona          | User Story Title                     | Priority (MoSCoW)   | MVP Scope?   |
|:---------|:-----------|:-----------------|:-------------------------------------|:--------------------|:-------------|
| RTM-041  | "O31-38    | Shuttle Operator | Real-Time Digital Passenger Manifest | Must                | Yes          |
|          |            |                  |                                      |                     |              |
|          | O31-14"    |                  |                                      |                     |              |

