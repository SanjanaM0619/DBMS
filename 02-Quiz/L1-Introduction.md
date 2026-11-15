# Lecture 01: Introduction to DBMS — Conceptual Quiz

### Q1. Relational Terminology
**Question:** If a relation (table) has **5 rows** and **4 columns**, how many **tuples** and how many **attributes** does it have?
* **Answer:** **5 tuples** (Cardinality = 5) and **4 attributes** (Degree = 4).

---

### Q2. Data Classification
**Question:** In a music streaming app, `username`, `subscription_plan`, and `join_date` are stored in a table, while `.mp3` audio files and `.jpg` album covers are stored separately. Which part is **structured data** and which is **unstructured data**?
* **Answer:**
  * **Structured Data:** `username`, `subscription_plan`, `join_date` (tabular format).
  * **Unstructured Data:** `.mp3` audio files, `.jpg` album covers (non-tabular media files).

---

### Q3. CRUD Mapping
**Question:** Which CRUD operation (**Create, Read, Update, or Delete**) maps to each of the following actions?
* Searching for all trains between Mangaluru and Bengaluru $\rightarrow$ **Read**
* Changing your registered email address on a portal $\rightarrow$ **Update**
* Registering a brand-new user account $\rightarrow$ **Create**

---

### Q4. RDBMS vs. DBMS Pioneer
**Question:** Why is **E.F. Codd** specifically called the *Father of RDBMS* rather than just the *Father of Databases* (Charles W. Bachman)?
* **Answer:** **Charles W. Bachman** pioneered early navigational databases (Network Data Model / CODASYL) that relied on physical pointers to traverse records. **E.F. Codd** (1970) introduced the **Relational Model**, representing all data mathematically as 2D tables (**Relations**) of rows and columns queried declaratively without physical pointers.