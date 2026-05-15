# 🚀 Project Name: dmoney-api-testing-postman

## 📝 Project Description

A comprehensive **API Integration Testing** repository for the **dMoney MFS** (Mobile Financial Service) core engine using **Postman**. 

This project validates critical banking workflows, ensuring security, data integrity, and compliance across various fintech operations.

### ✨ Key Testing Features Covered:
*   **Authentication Flow:** Validating two-step OTP logins for customers/agents and direct JWT generation for Admin accounts.
*   **Ledger Verification:** Checking the double-entry transaction database schema to ensure balance accuracy across credit and debit logs.
*   **Role-Based Access Control (RBAC):** Rigorous testing of unique workflows and endpoint permissions for Admin, Agent, Customer, Merchant, and SYSTEM roles.
*   **Boundary & Negative Testing:** Automated assertion logic checking input validation for string inputs in numeric fields (like Phone, NID) and handling unexpected payloads with proper error status codes ($400\text{ Bad Request}$, $401\text{ Unauthorized}$).

*   
