# Lecture 02: File System vs. DBMS — Application Scenario

## Scenario
A medical clinic stores patient prescriptions and billing details inside individual Word/CSV files organized by date folders (e.g., `2026-11-01/patient_101.csv`).

---

### 1. Atomicity & Power-Failure Recovery
* **File System Behavior:** If power cuts out midway while deducting an advance deposit and generating a receipt, the file is left partially written or corrupted, making it unclear which step succeeded.
* **DBMS Behavior:** Guarantees **Atomicity** (all-or-nothing execution). If a crash occurs before the transaction commits, the DBMS rolls back all partial changes to the exact state before the operation began.

---

### 2. Preventing Duplicate Patient Registrations
* **`patient_id` (`PRIMARY KEY`):** Uniquely identifies each patient record in the `PATIENTS` table.
* **`phone_number` (`UNIQUE` Constraint):** Prevents the same returning patient from accidentally being registered twice under two different auto-generated `patient_id` values.