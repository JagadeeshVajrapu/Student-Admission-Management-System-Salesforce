# Student-Admission-Management-System-Salesforce

Student Admission Management System (Salesforce)
📌 Project Overview

The Student Admission Management System is a Salesforce-based application built using Lightning Experience.

This project manages student admission records, automates approval notifications using Flow Builder, and provides real-time insights through Reports and Dashboards.

It demonstrates Salesforce configuration skills including custom objects, validation rules, automation, reporting, and dashboard creation.

🚀 Key Features
🏗 Custom Object

Student (Custom Object)

📝 Custom Fields

Student Name (Text)

Email (Email)

Phone (Phone)

Course (Picklist)

B.Tech

MBA

MCA

B.Sc

Status (Picklist)

Applied

Under Review

Approved

Rejected

Application Date (Date)

🔐 Validation Rule

A validation rule ensures:

Email field cannot be left blank.

Prevents saving incomplete student records.

Validation Logic Used:

ISBLANK(Email)
🔄 Automation (Flow Builder)

A Record-Triggered Flow is implemented:

Trigger: When Student record is created or updated

Condition: Status = Approved

Action: Automatically sends email notification to student

📧 Email Automation

When a student’s status changes to Approved,
an email is sent automatically to the student's email address.

📊 Reports
Student Admission Report

The report displays:

Student Name

Email

Course

Status

Application Date

Grouped By:

Course

Status

This allows tracking of:

Number of students per course

Number of approved/rejected students

📈 Dashboard
Student Admission Dashboard

The dashboard contains:

1️⃣ Students by Course (Pie Chart)
2️⃣ Students by Status (Bar Chart)

The dashboard updates automatically when new student records are added.

🧪 Testing Scenarios
✅ Test Email Automation

Create a new Student record

Set Status = Approved

Save record

Verify email received

✅ Test Report

Open Student Admission Report

Click Run

Confirm new student appears

✅ Test Dashboard

Open Dashboard

Click Refresh

Charts update automatically

🛠 Tools & Technologies Used

Salesforce Lightning Experience

Custom Objects & Fields

Validation Rules

Flow Builder (Record-Triggered Flow)

Reports & Dashboards
