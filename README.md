# 🏢 Employee and Project Management System (Zoho Creator)

## 📌 Overview

The **Employee and Project Management System** is a cloud-based business automation solution built using **Zoho Creator**, aimed at streamlining HR, project, and finance operations in an organization. This low-code application automates key workflows such as employee onboarding, department management, project proposal approvals, invoice generation, and leave request processing.

It features role-based access, real-time dashboards, Deluge-script-powered validations, email automation, and approval blueprints to ensure a smooth, efficient, and scalable organizational workflow.

---

## 🚀 Features

### 1. 🔐 User Roles & Permissions
- **Admin**: Full access to all modules.
- **Manager**: Can view and edit employee and project data.
- **Employee**: Can view and request access to their own data only.

### 2. 🧾 Forms & Modules
- **Department Form**  
  Captures department name (with uniqueness check), location, and head (lookup from Employee form).

- **Employee Form**  
  Captures name, auto-generated Employee ID (`ER0001`, `ER0002`...), email (validated), contact number, department (lookup), joining date, and reporting manager (lookup).

- **Project Proposal Form**  
  Captures project details, budget (positive only), submission date (not in past), manager (lookup), and team members via subform. Integrated with blueprint approval flow.

- **Invoice Form**  
  Auto-generates Invoice ID (`INV001`, `INV002`...), links to client and project, includes amount, due date, and status. Generates professional PDF templates and sends email to client.

- **Leave Request Form**  
  Captures leave type, start/end dates, and reason. Includes validations (date order, balance check), pop-up confirmation, and auto-email to reporting manager.

---

## 🧠 Business Logic & Validations (Deluge Scripting)

- **Auto-generation** of Employee & Invoice IDs.
- **Unique Checks** for department names and invoice numbers.
- **Date Validations** ensuring valid start/end/submission/due dates.
- **Field Format Validations** for emails and contact numbers.
- **Lookup Field Dependencies** dynamically pulling data from related forms.

---

## 📈 Reports & Dashboards

- **Employee Report**: Filterable by department and joining date.
- **Department Report**: All departments with head and location.
- **Project Proposal Report**: Shows current approval status.
- **Invoice Report**: Includes download button for PDF generation.
- **Leave Report**: Displays leave requests with status.

### 📊 Custom Dashboard Includes:
- Total number of:
  - Employees
  - Departments
  - Projects
  - Invoices
  - Leave Requests
- Charts:
  - Employee distribution by department
  - Project proposal status
  - Monthly invoice status
  - Leave requests by type and status

---

## 🔄 Approval Workflows & Automation

### ✅ Project Proposal Approval (Blueprint)
- **Stages**: Submitted → Under Review → Approved/Rejected
- Requires approval from both the Project Manager and Finance Head.

### 📧 Email Notifications
- **On Project Proposal Submission**: Sent to Project Manager & Finance Head
- **On Invoice Generation**: Sent to Client
- **On Leave Request Submission**: Sent to Reporting Manager

---

## 🧩 Widget
Custom dashboard widget for **Employee Leave Management**:
- Displays list of employees with leave balance
- Search bar to filter by name/department
- Button to apply for new leave

---

## 🛠 Technologies Used

| Technology | Description |
|------------|-------------|
| **Zoho Creator** | Low-code cloud development platform |
| **Deluge Script** | Logic and automation scripting |
| **Record Templates** | For PDF generation of invoices |
| **Blueprints** | For approval workflows |
| **Dashboards & Widgets** | Visual data representation |
| **Email Workflows** | Triggered notifications |

---

