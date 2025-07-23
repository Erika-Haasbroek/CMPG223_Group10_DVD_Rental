# CMPG223 Group 10 - DVD Rental System

This project was developed for the CMPG223 module at North-West University. It simulates the operations of a traditional DVD rental store, enabling staff to manage rentals, returns, customer data, and inventory — all via a custom-built C#.NET application backed by a Microsoft SQL Server 2022 database.

---

## 📋 Project Description

The system provides core functionality for a DVD rental business, such as:

- Managing customer information (add/update/remove)
- Registering new DVDs and genres
- Handling DVD rentals and returns
- Automatically calculating fines for late returns
- Viewing and managing rental history
- Ensuring data integrity through SQL database interactions

---

## ✅ Core Features

- 📀 **DVD Management**  
  Add, update, or remove DVDs and genres.

- 👤 **Customer Records**  
  Maintain complete customer profiles with history.

- 🕒 **Rental & Return Handling**  
  Process rentals, validate return dates, and handle overdue items.

- 💰 **Fine Calculation**  
  Auto-calculate fines based on configurable return windows.

- 📊 **Reports & Queries**  
  View rental history and current active rentals.

---

👥 Group 10 Members
- Francois Verster
- Rohann Venter
- Stefan Venter
- Christo Prinsloo
- Erika Haasbroek
- Jacques van Heerden (Maintainer of this fork)

---

## 💻 Technologies Used

- **Frontend / Application Layer:** C#.NET (WinForms)
- **Backend / Database:** Microsoft SQL Server 2022
- **IDE:** Visual Studio 2022
- **Database Tools:** SQL Server Management Studio (SSMS)
- **Version Control:** Git & GitHub

---

## ⚙️ Setup Instructions

### 1. Prerequisites

Ensure the following tools are installed:

- [Visual Studio 2022](https://visualstudio.microsoft.com/)
- [Microsoft SQL Server 2022](https://www.microsoft.com/en-us/sql-server)
- [SQL Server Management Studio (SSMS)](https://learn.microsoft.com/en-us/sql/ssms/)
- [Git](https://git-scm.com/) – for command-line version control
- [GitHub Desktop](https://desktop.github.com/) – optional, for GUI-based Git operations

> You will need either **Git** or **GitHub Desktop** to pull/push code to and from this repository.

---

### 2. Clone the Repository

Using GitHub Desktop:
- Open GitHub Desktop
- Click **"File" > "Clone repository"**
- Paste the repo URL:`https://github.com/JacquesNWU/CMPG223_Group10_DVD_Rental.git`

Using Git (CLI):
- git clone https://github.com/JacquesNWU/CMPG223_Group10_DVD_Rental.git
- cd CMPG223_Group10_DVD_Rental

---

### 3. Build the Solution

- Open the `.sln` file in Visual Studio.
- Restore NuGet packages if prompted.
- Build the solution via **Build > Build Solution**.

---

### 4. Set Up the Database

- Open SSMS and connect to your local SQL Server instance.
- Create a new database (e.g., `DVD_Rental_DB`)
- Run the SQL scripts (if provided) from the `/Database` folder to create tables and seed data.
- In the application config file (e.g., `App.config`), update the connection string:

```xml
<connectionStrings>
  <add name="DVDConnectionString" connectionString="Data Source=YOUR_SERVER_NAME;Initial Catalog=DVD_Rental_DB;Integrated Security=True" providerName="System.Data.SqlClient" />
</connectionStrings>


Let me know if you'd like the connection string section customised for SQL authentication or a named instance.
