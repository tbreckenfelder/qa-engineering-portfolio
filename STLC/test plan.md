## **Test Plan & Test Case Design**
**Test Object (System under test):**

**Webshop: https://grocerymate.masterschool.com/**

***I am using the previously formulated requirements as the basis for the test plan.***

---
## **1. Product Analysis**

**Objective: What is the goal of the product?**

- The main goal of the product is to expand the existing shop with 3 new functions (see below) and to ensure the smooth functionality of existing features.

**Target User Group (Stakeholders): Who uses the product? Who are the relevant stakeholders on the user side?**

- The product is aimed at new and existing users of the platform, regardless of age, and users aged 18 and over (alcoholic beverages).

**Hardware and Software Specifications:**
Devices with standard configurations will be used.

**Hardware Requirements:**

- Devices: PCs, laptops, smartphones, tablets
- Minimum requirements: 4 GB RAM, 2 GHz processor

**Software Requirements:**

- Operating systems: Windows, macOS, Android, iOS
- Browsers: Chrome, Firefox, Safari, Edge
- Dependencies: Backend services, third-party advertising services, payment gateways

**Existing Functionalities:**

What features does the product offer – both existing and planned?
- Registration and login
- Product search with sorting function (e.g., by price), product categorization
- Adding products to favorites
- Adding products to the shopping cart
- Order processing: Entering billing and shipping addresses, selecting payment method, calculating the total amount

**Planned Functionalities:**
- Product rating system
- Age verification for alcoholic beverages
- Changes to shipping costs
---

## **2. Draft Test Strategy**
**Test Scope: (Scope of Testing)**

**Included in the scope:**

- Registration & Login
- Age restriction for account creation
- Product search with sorting function (e.g., by price), product categorization
- Adding products to favorites
- Adding products to the shopping cart
- Order processing: Entering billing and shipping address, selecting payment method, calculating total amount

**Not included in the scope:**
- Backend database operations
- UI functions

**Planned Test Types:**

- Functional tests
- Regression tests
- Usability tests

**Risks, Problems, and Countermeasures:**

**Development delays**
- Countermeasure: Plan buffer time

**Missing test data**
- Countermeasure: Create test data (mock data)

**Resource bottlenecks**

- Countermeasure: Identify and schedule backup personnel

**Test logistics (Test Responsibilities):**

- Test Manager: Thomas Breckenfelder
- QA Engineer (Function & Regression): Thomas Breckenfelder
- QA Engineer (Usability): Thomas Breckenfelder
- End User for UAT (User Acceptance Test): Student

---

## **3. Definition of Test Objectives**
**Objectives:**

- *Functionality:* Ensure that new and existing functions work as intended
- *User Interface (GUI):* Verify usability, consistency, and error-free operation
- *Usability:* Evaluate user-friendliness and accessibility

**Expected Results:**

- All existing and new functions behave according to the specification
- The interface is intuitive, responsive, and error-free
- The application is easy for end users to use; erroneous user input is displayed accordingly

---

## **4. Defining Test Criteria**
**Exit Criteria:**

- **All planned tests**: were executed
- **Execution Rate**: 100% of all test cases were executed
- **Pass Rate**: At least 90% of the executed test cases passed
- All critical and high-priority defects are closed
- The User Acceptance Test (UAT) was completed and released

**Suspension Criteria:**

- Critical errors that block the continuation of testing (Severity 1)
- Test environment failure (servers, database access)
- Lack of resources (tools, hardware, personnel)

**Continuation Criteria:**

- Release granted
- Required tools and personnel are available again
- Necessary test data has been created, corrected, or updated

---

## **5. Resource Planning**

- **Personnel**: QA team, development team, end users for UAT
- **Hardware:** PCs, laptops, tablets, smartphones
- **Software:** Current browsers (Chrome, Firefox, Safari, Edge), operating systems (Windows, macOS, Android, iOS)

- **Infrastructure:** Test environments, automation tools, performance testing tools
---

## **6. Testumgebung planen**
**Testgeräte**: Realgeräte mit echten Betriebssystemen und Browsern zur realitätsnahen Simulation
- NB MacBook Air 13“/16/256
- OS Sequoia 15.6.1
- Browser: Chrome für Mac

**Umgebungen:** 
- Entwicklung (DEV)
- TEST (Test)
- Abnahme (ACC - Acceptance)

---

## **7. Schedule and Effort Estimate**



| Aktivität                                                    | Startdatum | Enddatum   | Umgebung | Verantwortlich | Geplanter Aufwand |
|--------------------------------------------------------------|------------|------------| -------- |----------------|-------------------|
| Testplanung                                                  | 06.11.2025 | 06.11.2025 | Alle     | TB             | 7 Stunden         |
| Testfalldesign                                               | 07.11.2025 | 07.11.2025 | Alle     | TB             | 7 Stunden         |
| Unittest (nur Erweiterungen)                                 | 08.11.2025 | 08.11.2025 | TEST     | TB             | 7 Stunden         |
| Integrationstest (Zusammenspiel der neuen Module)            | 09.11.2025 | 09.11.2025 | TEST     | TB             | 5 Stunden         |
| Systemtest                                                   | 10.11.2025 | 10.11.2025 | TEST     | TB             | 7 Stunden         |
| Teil-Regressions-Test (die von denÄnderungen betroffen sind) | 11.11.2025 | 11.11.2025 | ACC      | TB             | 3 Stunden         |
| Abnahmetest (UAT)                                            | 11.11.2025 | 11.11.2025 | TEST     | PB             | 2 Stunden         |
| Dokumentation                                                | 11.11.2025 | 12.11.2025 | ACC      | TB             | 2 Stunden         |


