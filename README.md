# Cobol_Portfolio
This is a collection of the cobol I've coded throughout the semester.

## 📋 Table of Contents

| Repository | Primary Tech | Category |
|------------|--------------|----------|
| [CALC2000](#CALC2000)           | COBOL/JCL | CIS352 Introduction to Enterprise Computing |
| [UTIL2000](#UTIL2000)           | COBOL/JCL | CIS352 Introduction to Enterprise Computing |
| [RPT3002](#RPT3002)             | COBOL/JCL | CIS352 Introduction to Enterprise Computing |
| [RPT5000](#RPT5000)             | COBOL/JCL | CIS352 Introduction to Enterprise Computing |
| [RPT6000](#RPT6000)             | COBOL/JCL | CIS352 Introduction to Enterprise Computing |
| [SEQ3002](#SEQ3002)             | COBOL/JCL | CIS352 Introduction to Enterprise Computing |



---

## 📁 Project Summaries

---

### CALC2000
**COBOL Future Value Calculator**
👤 Author: Aidan Dunbar | 📅 Date: 02/04/2026
🔗 [GitHub Profile](https://github.com/ADunbar5612)

- **Short Summary:** A COBOL program that calculates the future value of an investment using compound interest. The program runs the calculation three times, doubling the investment amount after each iteration.
- **Technologies Used:**
  - COBOL
  - JCL
  - z/OS Mainframe Environment
- **Key Learning Concepts:** Arithmetic operations in COBOL, looping with `PERFORM`, formatted output using numeric editing, and JCL job execution for compile and run.
- **Project Status:** ✅ Completed
- **Course / Self-Project:** CIS352 Introduction to Enterprise Computing
- **Program Details:**
  | Parameter | Value |
  |-----------|-------|
  | Initial Investment | $1,000 |
  | Number of Years | 10 |
  | Yearly Interest Rate | 5.5% |
  | Investment Doubling | Twice during execution |
- **Files:**
  - `CALC2000.cbl` – COBOL source program
  - **Thumbnail Screenshot:**
  > `![CALC2000 Screenshot](assets/calc2000-thumbnail.png)`
- **Repository Link:** [View CALC2000 on GitHub](https://github.com/ADunbar5612/Chapter1COBOLCalc)



[🔼 Back to TOC](#table-of-contents)

---

### UTIL2000
**COBOL Utility Billing System**
👤 Author: Aidan Dunbar
🔗 [GitHub Profile](https://github.com/ADunbar5612)

- **Short Summary:** A COBOL program that simulates a real-world utility billing system using a three-tier rate model. Processes multiple customer records and calculates electricity charges based on usage, plus a flat service fee.
- **Technologies Used:**
  - COBOL
  - JCL
  - z/OS Mainframe Environment
  - ISPF Editor
  - SDSF (job output monitoring)
- **Key Learning Concepts:** Conditional logic and tier segmentation, multi-record processing, fixed-value data initialization, mainframe dataset and member management, ISPF terminal workflow, and GitHub version control.
- **Project Status:** ✅ Completed
- **Course / Self-Project:** CIS352 Introduction to Enterprise Computing
- **Billing Structure:**
  | Tier | Usage Range | Rate |
  |------|-------------|------|
  | Tier 1 | First 500 kWh | $0.12/kWh |
  | Tier 2 | 501–1000 kWh | $0.15/kWh |
  | Tier 3 | Above 1000 kWh | $0.18/kWh |
  | Service Fee | Flat rate | $14.95/customer |
- **Thumbnail Screenshot:**
  > `![UTIL2000 Screenshot](assets/util2000-thumbnail.png)`
- **Repository Link:** [View UTIL2000 on GitHub](https://github.com/ADunbar5612/UTIL2000)
- [🔼 Back to TOC](#table-of-contents)

---

### RPT3002
**COBOL Sales Report Generator**
👤 Authors: [Ben Stearns](https://github.com/bstearns07) & [Aidan Dunbar](https://github.com/ADunbar5612) | 📅 Last Updated: 03/19/2026
🔗 [GitHub Repository](https://github.com/ADunbar5612/RPT3002)

- **Short Summary:** A COBOL program that reads a customer master file and generates a professionally formatted Year-To-Date (YTD) sales report. Outputs customer details, current and previous year sales, dollar change, percentage change, and grand totals across all customers.
- **Technologies Used:**
  - COBOL (Enterprise COBOL 6.4)
  - JCL
  - z/OS Mainframe Environment
  - Visual Studio Code + Zowe Explorer
  - Partitioned Datasets (PDS)
- **Key Learning Concepts:** Control-break logic for branch grouping, subtotals and group aggregation, state tracking with control fields, multi-level report design (detail → subtotal → grand total), and edge case handling for divide-by-zero in financial calculations.
- **New Topics Covered:**
  - 🔀 Control Break Processing (branch change detection)
  - 📊 Subtotals & Group Aggregation (branch-level totals)
  - 🧠 State Tracking using control fields (`OLD-BRANCH-NUMBER`)
  - 🔄 Conditional Output Formatting (suppressing repeated values)
  - ➗ Advanced error handling (`ON SIZE ERROR`, divide-by-zero cases)
- **Project Status:** ✅ Completed
- **Course / Self-Project:** CIS352 Introduction to Enterprise Computing
- **Files:**
  | File | Description |
  |------|-------------|
  | `RPT3000.cbl` | COBOL source program |
  | `JCLRPT3.jcl` | JCL used to compile and execute program |
  | `README.md` | Project documentation |
- **Thumbnail Screenshot:**
  > `![RPT3000 Screenshot](assets/rpt3000-thumbnail.png)`
- **Repository Link:** [View RPT3000 on GitHub](https://github.com/ADunbar5612/RPT3002)

[🔼 Back to TOC](#table-of-contents)
---

### RPT5000
**COBOL Sales Report Generator (Enhanced)**
👤 Author: [Aidan Dunbar](https://github.com/ADunbar5612) | 📅 March 31, 2026
🔗 [GitHub Repository](https://github.com/ADunbar5612/RPT5000)

- **Short Summary:** An enhanced version of RPT3000 that adds Sales Representative-level control breaks, improved branch totals, and grand total accumulation. Produces a fully structured multi-level YTD sales report with clean formatting and edge case handling.
- **Technologies Used:**
  - COBOL (Enterprise COBOL 6.4)
  - JCL
  - z/OS Mainframe Environment
  - Visual Studio Code + Zowe Explorer
- **Key Learning Concepts:** Multi-level control break logic (SALESREP → BRANCH → Grand Total), `EVALUATE`-based decision handling, switch-based control flow, modular paragraph design, and divide-by-zero protection in financial calculations.
- **Project Status:** ✅ Completed
- **Course / Self-Project:** CIS352 Introduction to Enterprise Computing
- **Thumbnail Screenshot:**
  > `![RPT5000 Screenshot](assets/rpt5000-thumbnail.png)`
- **Repository Link:** [View RPT5000 on GitHub](https://github.com/ADunbar5612/RPT5000)

[🔼 Back to TOC](#table-of-contents)
---

### RPT6000
**COBOL Advanced Table Lookups & Data Internalization**
👤 Author: [Aidan Dunbar](https://github.com/ADunbar5612)
🔗 [GitHub Repository](https://github.com/ADunbar5612/RPT6000)
- **Short Summary:** An enterprise-grade COBOL reporting program that builds on RPT5000 by introducing dynamic table lookups, data internalization via `COPY` members, and advanced memory management. Reads a secondary `SALESREP` file into an internal table to dynamically match rep IDs to names in the final report.
- **Technologies Used:**
  - COBOL (Enterprise COBOL 6.4)
  - JCL
  - z/OS Mainframe Environment
  - Visual Studio Code + Zowe Explorer
  - `COPY` Members (external record definitions)
- **Key Learning Concepts:** Internal table processing with `OCCURS` and `SEARCH`/`INDEXED BY`, data internalization using `COPY` statements, `PACKED-DECIMAL` (`COMP-3`) for optimized mainframe storage, `REDEFINES` clause for special case handling, `EVALUATE TRUE` structures, and `ON SIZE ERROR` overflow protection.
- **Key Enhancements over RPT5000:**
  | Enhancement | Description |
  |-------------|-------------|
  | 🔎 Table Lookups | `SEARCH` verb maps SALESREP IDs to names dynamically |
  | 📦 COPY Members | External record definitions for `CUSTMAST` and `SALESREP` |
  | ⚡ COMP-3 Fields | `PACKED-DECIMAL` for optimized storage and performance |
  | 🛡️ REDEFINES | Displays `OVRFLW` or `N/A` when calculations aren't possible |
  | 🔀 EVALUATE TRUE | Replaces nested IF statements for cleaner control flow |
- **Project Status:** ✅ Completed
- **Course / Self-Project:** CIS352 Introduction to Enterprise Computing
- **Thumbnail Screenshot:**
  > `![RPT6000 Screenshot](assets/rpt6000-thumbnail.png)`
- **Repository Link:** [View RPT6000 on GitHub](https://github.com/ADunbar5612/RPT6000)

[🔼 Back to TOC](#table-of-contents)


