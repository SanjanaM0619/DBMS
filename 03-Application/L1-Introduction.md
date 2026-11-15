# Lecture 01: Introduction to DBMS — Application Scenario

## Scenario
A college fest organizing committee currently manages participant registrations, event schedules, and volunteer contact details using **15 different Excel spreadsheets** shared over WhatsApp.

---

### Part 1: Problems with Spreadsheet-Based Management
If a student changes their phone number or two coordinators edit the schedule simultaneously, the committee faces four major issues:
1. **Data Redundancy:** The same participant's details are duplicated across multiple event spreadsheets.
2. **Data Inconsistency:** Updating a student's phone number in a few sheets while missing others leaves conflicting contact details across files.
3. **Lack of Central Tracking:** It becomes difficult to identify which spreadsheet holds the latest, verified version of the data.
4. **Concurrency & Manual Overhead:** Manually editing 15 separate files is time-consuming, and simultaneous edits over WhatsApp cause coordinators to overwrite each other's changes.

---

### Part 2: Relational Schema Breakdown (Entities & Attributes)
Converting the fest's structured data into an RDBMS separates each real-world entity into its own distinct table with dedicated attributes:

| Entity (Table Name) | Attributes (Columns) |
| :--- | :--- |
| **`PARTICIPANTS`** | `usn`, `full_name`, `college_name`, `dept`, `email`, `phone_number` |
| **`EVENTS`** | `event_id`, `event_name`, `venue`, `start_time`, `registration_fee` |
| **`VOLUNTEERS`** | `volunteer_id`, `volunteer_name`, `assigned_event`, `shift_time` |
| **`SPONSORS`** | `sponsor_id`, `company_name`, `tier`, `contribution_amount` |