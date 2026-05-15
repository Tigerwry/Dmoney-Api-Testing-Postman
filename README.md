# 🚀 Project Name: dmoney-api-testing-postman

## 📝 Project Description

A comprehensive **API Integration Testing** repository for the **dMoney MFS** (Mobile Financial Service) core engine using **Postman**. 

This project validates critical banking workflows, ensuring security, data integrity, and compliance across various fintech operations.

### ✨ Key Testing Features Covered:
*   **Authentication Flow:** Validating two-step OTP logins for customers/agents and direct JWT generation for Admin accounts.
*   **Ledger Verification:** Checking the double-entry transaction database schema to ensure balance accuracy across credit and debit logs.
*   **Role-Based Access Control (RBAC):** Rigorous testing of unique workflows and endpoint permissions for Admin, Agent, Customer, Merchant, and SYSTEM roles.
*   **Boundary & Negative Testing:** Automated assertion logic checking input validation for string inputs in numeric fields (like Phone, NID) and handling unexpected payloads with proper error status codes ($400\text{ Bad Request}$, $401\text{ Unauthorized}$).
---

### 🧪 Phase 2: Executing the API Integration Test Suite

With your backend infrastructure up and running safely, you can execute the automated QA integration suites using either **Postman Desktop UI** or directly from the **VS Code Terminal via Newman (CLI)**.

#### 🎛️ Option A: Running via Postman Desktop Client (Visual GUI)
1. **Launch Postman:** Open the Postman desktop application on your system.
2. **Import Test Workspace:** Click on the **Import** button in the top-left section. Select the collection JSON file (`dmoney_api_collection.json`) and the environment configurations file from the `postman/` directory of this project.
3. **Set Active Environment:** Navigate to the top-right environment selector dropdown and toggle your imported environment (ensure the `baseUrl` property is mapped to `http://localhost:5000`).
4. **Trigger Collection Runner:** Click on the triple-dot menu (`...`) next to the imported dMoney Collection and select **"Run collection"**.
5. **Analyze Results:** Click the **"Run dMoney MFS Automation Suite"** button. The Postman sandbox engine will execute all endpoints sequentially and output visual verification loops for response headers, schemas, and assertions ($200\text{ OK}$, $400\text{ Bad Request}$).

#### 💻 Option B: Running via VS Code Terminal (Newman CLI Automation)
If you prefer real-time automated console execution directly inside your VS Code terminal (similar to a CI/CD pipeline flow), follow these instructions:

1. **Install Newman Framework:** Open a clean terminal in VS Code and install Postman's CLI runner globally on your machine:
   ```bash
   npm install -g newman

   ---

### 🔗 Project Deliverables & QA Artifacts

To review the detailed test planning, execution logs, and live tracking sheets, access the verified links below:

*   **🌐 Live API Documentation:** [View Postman Live API Docs](https://documenter.getpostman.com/view/54449251/2sBXqQHJFt)
    > *Interactive schema visualization featuring request bodies, authentication tokens, and mock response validation layers.*
*   **📊 Test Cases & Bug Report Sheet:** [Access Excel QA Artifacts on Google Drive](https://docs.google.com/spreadsheets/d/1VvECVtzLRhYOCI5w9wVFYiSa_amjrFP-Hr8d6QQze4I/edit?usp=sharing)
    > *Comprehensive Excel sheet documenting all API Test Cases mapped directly according to their Postman endpoint paths, along with a dedicated log of all identified bugs and defects discovered during testing.*
