# Lecture 01: Introduction to DBMS

* **Father of Databases:** Charles W. Bachman
* **Father of RDBMS:** Edgar Frank "Ted" Codd

---

## 1. Database
A **database** is a collection of **related data** that represents some aspect of the real world.

---

## 2. Types of Data: Structured vs. Unstructured

| Feature | Structured Data | Unstructured Data |
| :--- | :--- | :--- |
| **Definition** | Data organized and stored in a strict tabular/relational format. | Data that does not follow a predefined tabular schema or relational format. |
| **Structure** | Stored as **Relations (Tables)** made up of **Rows (Tuples)** and **Columns (Attributes)**. | Stored in raw, native file formats without fixed rows and columns. |
| **Ease of Querying** | Easily queried and analyzed using standard **SQL**. | Requires specialized tools, parsers, or NoSQL/object storage to process. |
| **Real-World Examples** | IRCTC railway records, University student databases, Hospital patient records. | Web pages (HTML), photos (`.jpg`), videos (`.mp4`), audio files (`.mp3`). |

---

## 3. Database Management System (DBMS)
A **DBMS** is a collection of software programs that enables users to efficiently create, define, and maintain a database.

* **Core Operations (CRUD):**
  * **C**reate — Inserting new records or creating database structures.
  * **R**ead — Retrieving or querying existing data.
  * **U**pdate — Modifying existing records.
  * **D**elete — Removing obsolete or unwanted records.
* **Popular RDBMS Software:** Oracle, MySQL, Microsoft SQL Server, IBM DB2.