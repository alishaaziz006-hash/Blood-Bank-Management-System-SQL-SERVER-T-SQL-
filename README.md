# Blood-Bank-Management-System-SQL-SERVER-T-SQL-
The **Blood Bank Management System** is a database-driven project designed to manage donor, recipient, hospital, and blood inventory information efficiently.
It is built using **Microsoft SQL Server** with full implementation of advanced **Database Administration & Management** concepts.  
Developed as part of the **Database Administration & Management Lab Project** at **University of Management and Technology (UMT)**, it demonstrates real-world use of triggers, stored procedures, views, indexes, and complex JOIN queries in T-SQL.

---

## 🎯 Features
- 🧑‍⚕️ Manage donor and recipient records with full details  
- 🏥 Track hospital requests and blood unit allocations  
- 🩸 Monitor blood inventory availability and expiry dates  
- 🔬 Quality control module for contamination tracking  
- ⚡ Trigger to auto-update blood availability on new requests  
- 📦 Stored procedures for reusable and secure data operations  
- 👁️ Views for simplified reporting and data abstraction  
- 📊 Indexes for optimized query performance  
- 🔗 Complex JOIN reports for full transfusion traceability  

---

## 🛠️ Tools & Technologies
- **Database Server:** Microsoft SQL Server  
- **Management Tool:** SQL Server Management Studio (SSMS)  
- **Query Language:** T-SQL (Transact-SQL)  
- **Operating System:** Windows OS  

---

## ⚙️ Setup Instructions
1. Install **Microsoft SQL Server** and **SQL Server Management Studio (SSMS)**.  
2. Open SSMS and connect to your SQL Server instance.  
3. Open the file `Blood_Bank_Management_System_SQL.sql` in SSMS.  
4. Press **F5** or click **Execute** to run the full script.  
5. The script will automatically create the database, tables, sample data, triggers, procedures, views, and indexes.  

> ⚠️ The script is safe to re-run — it checks for existing objects before dropping them.

---

## 🧩 File Structure

```
Blood-Bank-Management-System/
│
├── README.md                                               ← Project documentation
├── Blood_Bank_Management_System_SQL.sql                    ← Full T-SQL database code
├── Database_Administration_and_Management_Lab_Project.pdf  ← Project report
│
└── screenshots/
    ├── Donor_Table_Output.PNG
    ├── Blood_Inventory_Output.PNG
    ├── Hospital_Request_Output.PNG
    ├── Stored_Procedure_Output.PNG
    └── Views_Output.PNG
```

---

## 🗄️ Database Schema

| Table | Description |
|-------|-------------|
| `Donor` | Stores donor personal info, blood group, and disease status |
| `Hospital` | Registered hospitals that can request blood units |
| `Recipient` | Patients who need blood transfusions |
| `BloodInventory` | Tracks each blood unit's collection, expiry, and availability |
| `HospitalRequest` | Links hospitals, recipients, and blood units with request status |
| `QualityControl` | Records contamination test results per blood unit |

---

## ⚙️ DBA Concepts Implemented

| Concept | Details |
|---------|---------|
| 🔁 Trigger | `trg_UpdateAvailability` — auto-marks blood as "Used" on new request |
| 📦 Stored Procedures | `GetBloodByGroup` — fetch donors by blood group; `PendingRequests` — view pending hospital requests |
| 👁️ Views | `vw_AvailableBlood` — available blood units; `vw_HealthyDonors` — eligible donors |
| 📊 Indexes | `idx_Donor_BloodGroup` on Donor; `idx_Blood_Availability` on BloodInventory |
| 🔗 JOIN Report | Multi-table JOIN linking Donors → Inventory → Requests → Hospitals → Recipients |

---

## 📸 Output Screenshots

<details>
<summary>Click to view output screenshots</summary>

### Donor Table
![Donor Table](screenshots/Donor_Table_Output.PNG)

### Blood Inventory
![Blood Inventory](screenshots/Blood_Inventory_Output.PNG)

### Hospital Request (JOIN Report)
![Hospital Request](screenshots/Hospital_Request_Output.PNG)

### Stored Procedure Output
![Stored Procedure](screenshots/Stored_Procedure_Output.PNG)

### Views Output
![Views](screenshots/Views_Output.PNG)

</details>

---

## 👥 Group Members

| Registration # | Name |
|----------------|------|
| F2023105199 | Hassna Imtiaz |
| F2023105162 | Alisha Aziz |
| F2023105184 | Ayesha Zulfiqar |
| F2023105180 | Areeba Rasheed |
| F2023105193 | Maryam Afzal |
| F2023105145 | Muhammad Mubeen |

---

## 🎓 Project Info

- **Project Advisor:** Muhammad Amir Waseem  
- **Institution:** University of Management and Technology (UMT)  
- **Department:** Faculty of Informatics, School of Systems and Technology  
- **Subject:** Database Administration & Management Lab  

---

## 📄 License
This project was developed for academic purposes only.  
All rights reserved by the group members and UMT.

