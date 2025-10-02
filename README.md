# Employee-Scheduling-System

Great — thanks for sharing your notes! I’ll turn your sketch into a **clear description of the website** and then give you a **layout structure (like a sitemap + wireframe idea)**.

---

## 📌 Website Description: Employee Scheduling System

This website is designed for **managers** and **employees** to manage and view work schedules, availability, and time-off requests. It has two main user roles:

### 🔹 Manager View

Managers have full control over employee scheduling:

* **Add Employee** – Create new employee accounts.
* **Remove Employee** – Delete existing employee accounts.
* **Modify Availability** – Adjust employee availability if needed.
* **Modify Time Off** – Approve or edit employee time-off requests.
* **View/Modify Schedule** – Create, update, and manage shift schedules.
* **Add/Remove Shifts** – Assign shifts to employees or remove shifts.
* **Print or Email Schedule** – Share schedules with employees.

### 🔹 Employee View

Employees can manage their own availability and schedules:

* **View Schedule** – See their assigned shifts.
* **Update Availability** – Change availability preferences.
* **Request Time Off** – Submit time-off requests.

### 🔹 Dashboard (Shared Login System)

* **Login with UserID & Password**
* Based on role (Manager or Employee), the user is directed to their respective dashboard.

---

## 📌 Website Layout (Wireframe / Sitemap)

### 1. **Login Page**

* Fields: `UserID`, `Password`
* Buttons: `Login`
* Redirect:

  * If **Manager** → Manager Dashboard
  * If **Employee** → Employee Dashboard

---

### 2. **Manager Dashboard**

**Sections / Buttons:**

1. **Employee Management**

   * ➕ Add Employee
   * ➖ Remove Employee
2. **Schedule Management**

   * View Schedule
   * Add Shift
   * Remove Shift
   * Modify Availability / Time Off
   * Print/Email Schedule
3. **Quick Actions**

   * Approve Time Off Requests
   * Update Employee Records

---

### 3. **Employee Dashboard**

**Sections / Buttons:**

1. **My Schedule**

   * View Assigned Shifts
2. **My Availability**

   * Update Availability
3. **Time Off Requests**

   * Request Time Off
   * View Status of Requests

---

## 📌 Suggested Page Flow (Navigation)

```
Login Page
   ├── Manager Dashboard
   │       ├── Employee Management
   │       │      ├── Add Employee
   │       │      └── Remove Employee
   │       ├── Schedule Management
   │       │      ├── View/Modify Schedule
   │       │      ├── Add Shift
   │       │      └── Remove Shift
   │       ├── Print/Email Schedule
   │       └── Approve Time Off
   │
   └── Employee Dashboard
           ├── View Schedule
           ├── Update Availability
           └── Request Time Off
```

---

Got it 👍 You want a **website wireframe plan** that shows:

* **Navbar contents**
* **Home page layout**
* **How the website workflow will function**
* **Role-based permissions (Admin > Manager > Employee)**

Let’s build this step by step 👇

---

# 📌 Website Wireframe Plan

## 1. Navbar (Top Navigation Bar)

The navbar should change based on who is logged in (Admin, Manager, Employee).

🔹 **Before Login (Public User)**

* Home
* About
* Login
* Contact

🔹 **Admin Logged In**

* Dashboard
* Manage Managers (Create / Remove)
* Manage Employees
* Manage Schedules
* Reports
* Logout

🔹 **Manager Logged In**

* Dashboard
* Employees (Add / Remove / Availability / Time Off)
* Schedule (Create / Edit / Delete Shifts)
* Notifications (Time off requests, approvals)
* Logout

🔹 **Employee Logged In**

* My Schedule
* My Availability
* Request Time Off
* Profile
* Logout

---

## 2. Home Page Layout

**Sections:**

1. **Header (Navbar + Logo)**

   * Top navigation bar as above

2. **Hero Section**

   * Title: *"Smart Employee Scheduling System"*
   * Button: *Login*

3. **Features Section**

   * Cards (3–4 columns):

     * Easy Scheduling
     * Time-Off Management
     * Role-Based Access
     * Notifications

4. **How It Works (Steps)**

   * Step 1: Admin creates Managers
   * Step 2: Managers create Employees & Shifts
   * Step 3: Employees view schedules & request time off

5. **Contact / Support Section**

   * Email / Phone / Support Form

6. **Footer**

   * Links: Privacy Policy | Terms | Help

---

## 3. Workflow (Role-Based Power)

🔹 **Admin**

* Can **only** create and manage Managers.
* Can deactivate/activate managers.
* Has overall control of system reports.

🔹 **Manager**

* Created by Admin.
* Can add/remove employees.
* Can create/edit/delete schedules.
* Can approve/reject time-off requests.

🔹 **Employee**

* Created by Manager.
* Can only update their availability.
* Can view their schedule.
* Can request time off.

---

## 4. Wireframe Flow (Page Navigation)

```
Home Page
   ├── Login
   │      ├── Admin Dashboard
   │      │      ├── Manage Managers
   │      │      └── Reports
   │      │
   │      ├── Manager Dashboard
   │      │      ├── Manage Employees
   │      │      ├── Manage Schedule
   │      │      └── Approve Time Off
   │      │
   │      └── Employee Dashboard
   │             ├── My Schedule
   │             ├── My Availability
   │             └── Request Time Off
   │
   └── Contact Page


