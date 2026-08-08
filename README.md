# 🎓 Smart Campus Management System (SCMS)

> An enterprise-grade automation and university administration solution built on the ServiceNow platform (Vancouver Release).

---

## 🚀 Overview

The Smart Campus Management System replaces fragmented administrative paperwork and manual workflows with a centralized, secure self-service platform. Designed within an isolated scoped application container, the system seamlessly handles relational academic records, automated operational requests, and real-time administrative analytics.

---

## 🛠️ Problem Statement & Architecture

### **The Problem**
Traditional campus management relies on disconnected spreadsheets and manual data entry, leading to data silos, delays in student leave/complaint processing, and a lack of centralized operational oversight.

### **The Solution**
An end-to-end server-side and workflow-driven solution built entirely inside ServiceNow:
* **Scoped Application Isolation:** Securely housed within namespace `x_2065601_smart_0` to ensure proper data encapsulation and namespace integrity.
* **Relational Data Schema:** Structured master and transactional tables linking departments, courses, students, faculty, enrollments, and operational complaints.
* **Automated Processing:** Dynamic UI policies, data-integrity business rules, and asynchronous Flow Designer workflows.

---

## 📂 Core Architecture & Components

### **1. Data Model (Tables)**
* **Academic Master Tables:** Departments, Courses, Students, Faculty.
* **Operational Transactional Tables:** Course Enrollments, Leave Requests, Facility Complaints.

### **2. Logic & Automation**
* **Script Includes (`scmsutils`):** Reusable backend scripts handling server-side processing and data validation.
* **Client Scripts & UI Policies:** Real-time form validations and dynamic field visibility rules.
* **Auto-Numbering Generators:** Systematic tracking IDs for complaints and requests.

### **3. Service Portal & Workflows**
* **Service Catalog:** User-friendly self-service portal landing page (`Smart Campus Services`) for students and faculty.
* **Flow Designer:** Automated multi-step approval routing and automated email status notifications.

---

## 📊 Administrative Dashboards & Reporting
* Real-time graphical reporting tracking:
  * Course enrollment trends across academic terms.
  * Open leave request backlogs.
  * Facility complaint distributions by category.

---

## 📦 Project Deployment
* Packaged completely as a standard ServiceNow **Update Set**, ensuring seamless migration and deployment across instances.

---

## 🔗 Project Documentation
* For a comprehensive deep-dive into the technical implementation, schemas, and walkthrough, check out the documentation folder in this repository:
  👉 **[View Project Documentation PDF]([[./6.%20Project%20Documentation/ServiceNow_Capstone_Documentation.pdf](https://github.com/santhoshakkisetti/Smart-Campus-Management-System/blob/main/6.%20Project%20Documentation/ServiceNow_Capstone_Documentation().pdf)](https://github.com/santhoshakkisetti/Smart-Campus-Management-System/blob/main/6.%20Project%20Documentation/ServiceNow_Capstone_Documentation().pdf))**
