# HCl AutoQA: E-Commerce Automation Framework

## Project Overview
This repository contains a professional **Selenium-Java** automation framework developed for the HCL Hackathon. The framework automates a complete end-to-end user journey on the **Automation Exercise** website, encompassing the full lifecycle from account creation to final order payment.

The architecture strictly follows the **Page Object Model (POM)** to ensure high maintainability, code reusability, and scalability.

---

## Project Execution Timeline
This project was developed in an intensive 24-hour agile development cycle:

* **Phase 1 (Morning):** Requirement analysis, Maven project setup, and development of the `BasePage` and `BaseTest` core utilities.
* **Phase 2 (Afternoon):** Implementation of **Authentication Module** featuring dynamic email generation for repeatable testing.
* **Phase 3 (Evening):** Development of **Product Search** and **Cart Management** modules. Integration of TestNG Listeners.
* **Phase 4 (Final):** Completion of **Checkout & Payment** logic, integration of **Extent Reports (Spark)**, and final documentation.

---

## Technical Features
* **Design Pattern:** Page Object Model (POM) for clear separation of UI elements and test logic.
* **Reporting:** Extent Reports (Spark) providing a graphical dashboard of test execution results.
* **Synchronization:** Optimized performance using **Explicit Waits (WebDriverWait)** instead of static sleeps.
* **Configuration:** Centralized management of environment variables via `config.properties`.
* **Error Handling:** Automatic screenshot capture triggered by TestNG Listeners on test failure.

---

## Project Structure
The project is organized into the following package structure:

* `src/main/java/com/autoqa/pages`: Contains locators and action methods for each web page.
* `src/main/java/com/autoqa/utils`: Shared utility classes (e.g., `ConfigReader`, `TestListener`).
* `src/test/java/com/autoqa/tests`: TestNG execution scripts for end-to-end scenarios.
* `reports/`: Storage for the generated `ExtentReport.html`.
* `screenshots/`: Captured visual evidence of test execution and order confirmations.

---

## Tech Stack
* **Language:** Java 11+
* **Automation Tool:** Selenium WebDriver 4.x
* **Test Runner:** TestNG
* **Reporting Tool:** Extent Reports
* **Build Management:** Maven

---

## Installation and Execution
Follow these steps to run the automation suite locally:

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/dhathri25/HCl-AutoQA-ECommerce-Website-Project1.git](https://github.com/dhathri25/HCl-AutoQA-ECommerce-Website-Project1.git)
    ```
2.  **Environment Setup:**
    Ensure Java 11+ and Apache Maven are installed and configured in your system path.
3.  **IDE Import:**
    Import the project as a **Existing Maven Project** into Eclipse or IntelliJ IDEA.
4.  **Run Tests:**
    Right-click on the `testng.xml` file and select **Run As > TestNG Suite**.
5.  **View Results:**
    Navigate to the `reports/` folder and open `ExtentReport.html` in any web browser.

---
*Developed by Dhathri Putty for the HCL Hackathon.*