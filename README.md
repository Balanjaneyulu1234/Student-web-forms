```markdown
# 📘 StudentWebApp

A simple **Student Management Web Application** built with **ASP.NET Core MVC** and **Entity Framework Core**.  
This app allows you to **add, view, edit, and delete student records** in a SQL Server database.  

---

## 🚀 Features
- View a list of students  
- Add new student details  
- Edit existing student records  
- Delete students  
- View detailed information of a student  

---

## 🛠️ Tech Stack
- **ASP.NET Core 7.0** (MVC Framework)  
- **Entity Framework Core** (ORM)  
- **SQL Server** (Database)  
- **Bootstrap 5** (UI Styling)  
- **HTML, CSS, JavaScript** (Frontend)  

---

## 📂 Project Structure
```

StudentWebApp/
┣ Controllers/
┃ ┗ StudentsController.cs  

# Handles CRUD logic
┣ Models/
┃ ┗ Student.cs  

# Student model
┣ Data/
┃ ┗ ApplicationDbContext.cs 

# EF Core DbContext
┣ Views/
┃ ┣ Shared/
┃ ┃ ┗ \_Layout.cshtml  

# Common layout
┃ ┣ Students/
┃ ┃ ┣ Index.cshtml               # List students
┃ ┃ ┣ Create.cshtml  

# Add student
┃ ┃ ┣ Edit.cshtml                # Update student
┃ ┃ ┣ Details.cshtml 

# View details
┃ ┃ ┗ Delete.cshtml              # Delete student
┣ wwwroot/
┃ ┣ css/site.css                 # Custom CSS
┃ ┣ js/site.js                   # Custom JS
┃ ┗ lib/bootstrap/               # Bootstrap (optional if using CDN)
┣ Program.cs                     

# Application entry point
┗ appsettings.json                # Database configuration

````

---

## ⚙️ Setup and Run Instructions

### ✅ Prerequisites
- [Visual Studio 2022](https://visualstudio.microsoft.com/downloads/)  
- [.NET 7.0 SDK](https://dotnet.microsoft.com/en-us/download/dotnet/7.0)  
- [SQL Server 2019/2022](https://www.microsoft.com/en-us/sql-server/sql-server-downloads)  
- [SQL Server Management Studio (SSMS)](https://aka.ms/ssmsfullsetup)  

---

### 🔧 1. Clone or Create the Project
```bash
git clone https://github.com/your-username/StudentWebApp.git
cd StudentWebApp
````

---

### 🛠️ 2. Configure Database

Open **appsettings.json** and set your connection string:

```json
"ConnectionStrings": {
  "DefaultConnection": "Server=localhost;Database=StudentDB;Trusted_Connection=True;TrustServerCertificate=True;"
}
```

---

### 🗃️ 3. Apply Migrations

```bash
dotnet tool install --global dotnet-ef   # if not installed
dotnet ef migrations add InitialCreate
dotnet ef database update
```

---

### ▶️ 4. Run the Application

```bash
dotnet run
```

Open in browser:
👉 `https://localhost:5001`
👉 `http://localhost:5000`

---

## 🎨 UI Styling

This project uses **Bootstrap 5**.

Using **CDN** (recommended):

```html
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
```

Or download [Bootstrap](https://getbootstrap.com/docs/5.3/getting-started/download/) and place inside `wwwroot/lib/bootstrap/`.

---

## 📸 Screenshots

* **Home Page (Index)** → Shows list of students
* **Create Page** → Add new student
* **Edit Page** → Update student details
* **Details Page** → View student information
* **Delete Page** → Confirm delete

---

## 🧑‍💻 Author

👤 TIRUPATHI BALANJANEYULU 
📧 balanjaneyulu100@gmail.com
🔗 GitHub : https://github.com/Balanjaneyulu1234
