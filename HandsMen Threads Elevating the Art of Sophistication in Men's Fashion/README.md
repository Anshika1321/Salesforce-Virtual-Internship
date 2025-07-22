# 📘 HandsMen Threads CRM Implementation

## 📌 Project Title

**HandsMen Threads: Elevating the Art of Sophistication in Men's Fashion with Salesforce CRM**

---

## 📝 Overview

This project involves the development and deployment of a **custom Salesforce CRM** tailored for **HandsMen Threads**, a premium men’s fashion and tailoring brand.

The implementation enhances customer engagement, streamlines business processes, and maintains data integrity across departments (Sales, Inventory, and Marketing) using Salesforce’s declarative and programmatic capabilities.

---

## 🎯 Objectives

* Streamline operational processes (orders, inventory, customer records, campaigns).
* Maintain accurate and consistent data across all departments.
* Personalize customer experiences via loyalty tiers and targeted emails.
* Enable scalable automation and reporting for future growth.

---

## 🧰 Key Technologies Used

| Technology                   | Description                                                   |
| ---------------------------- | ------------------------------------------------------------- |
| **Salesforce CRM**           | Core platform for managing records, processes, and automation |
| **Flows**                    | Record-Triggered, Scheduled Flows to automate tasks           |
| **Apex**                     | Custom logic for triggers and batch jobs                      |
| **Validation Rules**         | Ensure clean and accurate data entry                          |
| **Email Alerts & Templates** | Automated notifications for orders, loyalty, inventory        |
| **Roles & Profiles**         | Secure, role-based access and collaboration                   |
| **Custom Objects**           | Five main objects tailored to business needs                  |

---

## 📦 Custom Objects

| Object Name        | Description                              |
| ------------------ | ---------------------------------------- |
| **Customer\_\_c**  | Stores customer details & loyalty status |
| **Product\_\_c**   | Product catalog with price, stock, SKU   |
| **Order\_\_c**     | Tracks orders with quantities and status |
| **Inventory\_\_c** | Manages stock levels per product         |
| **Campaign\_\_c**  | Stores marketing campaign data           |

---

## ⚙️ Features Implemented

### 🔁 Automation

* **Order Confirmation Flow** – Sends email when order is marked Confirmed.
* **Low Stock Alert Flow** – Notifies Inventory Manager when stock < 5.
* **Loyalty Status Flow** – Scheduled job updates loyalty level nightly.

### 💻 Apex Triggers

* `OrderTriggerHandler` – Manages multiple order-related triggers.
* Auto-calculate `Total_Amount__c` from quantity × unit price.
* Reduce inventory quantity on order.
* Loyalty updates based on total purchases.

### ✅ Validation Rules

* Email format (`@gmail.com`) for Customer\_\_c
* Prevent order amount ≤ 0
* Inventory quantity must be ≥ 0

### 📧 Email Templates

* Order Confirmation
* Low Stock Alert
* Loyalty Tier Update Notification

### 🔒 User Access

* **Roles:** Sales, Inventory, Marketing
* **Profiles:** Platform 1 profile with custom permissions
* **Users:**

  * Niklaus Mikaelson – Sales
  * Kol Mikaelson – Inventory

---

## 🧪 Sample Use Case Walkthrough

1. **Customer Siya Mikaelson registers**
   → Email is validated
2. **Admin adds 2 shirts @ ₹500 each**
   → Inventory is updated
3. **Siya places an order**
   → Triggers calculate total (₹1000), deduct stock
4. **Loyalty tier updated to Silver**
   → Email notification sent
5. **Stock alert triggers if quantity falls below 5**

---

## 🖼️ Visual Assets

* Custom App Interface
* Customer & Product Records
* Order Confirmation Screen
* Loyalty Tier Email
* Low Stock Alert Sample

*(Include screenshots if hosting this on GitHub or Salesforce DevHub)*

---

## 📈 Future Enhancements

* 🌐 **Customer Self-Service Portal**
* 📱 **Salesforce Mobile SDK App**
* 📊 **Dynamic Reports & Dashboards**
* 🤖 **AI Product Suggestions (Einstein AI)**
* 📲 **WhatsApp/SMS Integration for real-time updates**

---

## 🔧 Setup Instructions

1. **Sign up for Salesforce Developer Org**
   → [https://developer.salesforce.com/signup](https://developer.salesforce.com/signup)

2. **Deploy Metadata / Custom Objects**
   Use Salesforce Setup → Object Manager → New → Create objects & fields as defined.

3. **Build Lightning App**
   → App Manager → New Lightning App → Add Tabs for Custom Objects

4. **Create Users, Roles & Profiles**
   → Setup → Users → New → Assign based on department.

5. **Set Up Flows, Triggers & Email Alerts**
   → Use Flow Builder and Apex Classes/Triggers in Developer Console

---

## 🏁 Conclusion

The custom Salesforce CRM solution has transformed HandsMen Threads into a **data-driven, customer-centric business**. With automated workflows, real-time insights, and personalization, this implementation paves the way for **sustainable growth** and **scalable customer engagement**.

---


