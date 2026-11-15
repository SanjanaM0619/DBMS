# Lecture 02: File System vs. DBMS

A **File System** stores data in isolated flat files (e.g., `.txt`, `.csv`, `.xlsx`) managed by the OS, whereas a **DBMS** manages structured, interrelated data centrally with built-in integrity, security, and concurrency controls.

---

## Why DBMS is Better than a File System?

| Feature / Parameter | File System | DBMS |
| :--- | :--- | :--- |
| **1. Granular Data Access** | Requires loading or downloading the entire file to extract even a single record. | Fetches only the exact requested rows/columns via declarative queries (e.g., SQL). |
| **2. Search Mechanism (Metadata vs. Attributes)** | Searches rely primarily on **file metadata** (file name, folder path, modified date) rather than internal content. | Searches directly through **attributes (columns)** using indexing (e.g., `WHERE salary > 50000`). |
| **3. Concurrency Control** | Simultaneous edits by multiple users cause race conditions, file locks, or overwritten data. | Built-in concurrency protocols (locks, timestamps) allow safe simultaneous multi-user access. |
| **4. Security & Access Control** | Basic OS-level file permissions (all-or-nothing access to the entire file). | Granular **Role-Based Access Control (RBAC)** restricts access down to specific tables, rows, or columns. |
| **5. Data Redundancy** | High duplication across separate department files wastes storage. | Integrity constraints (`PRIMARY KEY`, `UNIQUE`, `FOREIGN KEY`) minimize duplicate records. |
| **6. Data Consistency** | High risk of **Data Inconsistency** (updating a record in one file leaves outdated copies in others). | Centralized storage and constraints keep data uniform and consistent across all views. |
| **7. Atomicity (Crash Recovery)** | No transaction support—a system crash mid-write leaves files partially updated or corrupted. | Guarantees **Atomicity** (all-or-nothing execution): failed operations roll back cleanly. |

---

## Key Exam Terms to Remember
* **Data Redundancy:** Unnecessary duplication of the same data across multiple places.
* **Data Inconsistency:** The direct consequence of redundancy—when multiple copies of the same data no longer match after a partial update.
* **Atomicity:** Ensuring a multi-step operation either completes 100% or fails completely with zero partial changes saved.