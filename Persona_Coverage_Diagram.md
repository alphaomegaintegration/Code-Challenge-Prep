# Persona Coverage Diagram
This diagram shows how each **persona** is covered across the solution epics. The edge labels reflect the number of RTM entries mapped from that persona to each epic.

## GitHub Mermaid Diagram

```mermaid
flowchart LR
    P_STU["Student"]
    P_ADM["Administrator"]
    P_OPR["Shuttle Operator"]
    E1["Epic 1 – Student Onboarding"]
    E2["Epic 2 – Integrated Search & Safe Transfer Booking"]
    E3["Epic 3 – Digital Boarding & Real-Time Tracking"]
    E4["Epic 4 – Booking Lifecycle & Notifications"]
    E5["Epic 5 – Student Engagement & Social Features"]
    E6["Epic 6 – Admin Operations Center"]
    E7["Epic 7 – Shuttle Operator Tools"]
    P_ADM -->|19 RTM item(s)| E6
    P_OPR -->|1 RTM item(s)| E7
    P_STU -->|6 RTM item(s)| E1
    P_STU -->|6 RTM item(s)| E2
    P_STU -->|3 RTM item(s)| E3
    P_STU -->|6 RTM item(s)| E4
    P_STU -->|5 RTM item(s)| E5
```

## Persona-to-Epic Coverage Table

| Persona          | Epic                                               |   RTM Count |
|:-----------------|:---------------------------------------------------|------------:|
| Administrator    | Epic 6 – Admin Operations Center                   |          19 |
| Shuttle Operator | Epic 7 – Shuttle Operator Tools                    |           1 |
| Student          | Epic 1 – Student Onboarding                        |           6 |
| Student          | Epic 2 – Integrated Search & Safe Transfer Booking |           6 |
| Student          | Epic 3 – Digital Boarding & Real-Time Tracking     |           3 |
| Student          | Epic 4 – Booking Lifecycle & Notifications         |           6 |
| Student          | Epic 5 – Student Engagement & Social Features      |           5 |

## Evaluator Readout

- **Student:** covered by **5 epic(s)** across **26 RTM item(s)**.
- **Administrator:** covered by **1 epic(s)** across **19 RTM item(s)**.
- **Shuttle Operator:** covered by **1 epic(s)** across **1 RTM item(s)**.