# Test Automation with Selenium WebDriver

## Objectives

- **Set Up Selenium WebDriver:**  
  Learn how to install and configure Selenium WebDriver with ChromeDriver for automated browser testing.  

- **Implement JUnit 5/TestNG for Test Execution:**  
  Use JUnit 5 or TestNG annotations to structure test cases effectively.  

- **Automate a Simple Web Test:**  
  Write and execute a basic UI test.  

- **Set Up Continuous Integration (CI):**  
  Configure a CI pipeline using GitHub Actions to automate Selenium tests.  

---

## Project: Selenium WebDriver Setup and Basic UI Testing

## Overview

This project focuses on setting up Selenium WebDriver, creating automated UI tests, applying design patterns like Page Object Model (POM), and integrating Continuous Integration using GitHub Actions.

---

## 1. Setup and Configuration

### Build Tools
- Maven or Gradle  

### Dependencies
Add the following dependencies to your `pom.xml`:

- Selenium WebDriver  
- JUnit 5 or TestNG  

---

## 2. Basic Automated Test

- Launch the **Newsletter Sign-Up Form**  
- Automate form submission using Selenium WebDriver  
- Validate successful submission using a success message  

---

## 3. Page Object Model (POM)

### Requirements

- Create separate **Page Classes** for each page  
- Use **locators** to identify UI elements  
- Implement **Page Factory Pattern** for better structure and maintainability  

---

## 4. Continuous Integration with GitHub Actions

### Workflow Setup

- Create a workflow file:  
