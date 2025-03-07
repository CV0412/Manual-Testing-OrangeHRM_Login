# OrangeHRM Login Manual Testing

Welcome to the **OrangeHRM Login Testing** repository! This project focuses on performing **manual testing** on the login functionality of the **OrangeHRM** demo platform. It covers various scenarios such as valid and invalid login attempts, password masking, field validation, and security testing like SQL injection.

This repository contains detailed test cases, test execution logs, bug reports, and a final summary of the testing process.

## Table of Contents

- [Overview](#overview)
- [Test Objectives](#test-objectives)
- [Test Approach](#test-approach)
- [Test Cases](#test-cases)
  - [Positive Test Cases](#positive-test-cases)
  - [Negative Test Cases](#negative-test-cases)
- [Test Execution](#test-execution)
- [Bug Reports](#bug-reports)
- [Test Summary Report](#test-summary-report)
- [How to Run Tests](#how-to-run-tests)
- [Technologies Used](#technologies-used)

---

## Overview

This project documents the manual testing of the **login functionality** for **https://opensource-demo.orangehrmlive.com/web/index.php/auth/login**. The goal is to ensure that users can log in securely and that the login page handles various scenarios gracefully, including **valid/invalid login attempts**, **empty fields**, **SQL injection attempts**, and proper **password masking**.

## Test Objectives

The primary objectives of this testing project are:

1. Validate that a user can successfully log in with valid credentials.
2. Ensure that the system prevents login attempts with invalid credentials (incorrect username or password).
3. Verify that the system handles empty field submissions (empty username or password) correctly.
4. Check that the login page properly masks the entered password for security.
5. Test the login page for **SQL injection vulnerabilities**.
6. Ensure the system responds appropriately to all edge cases and unexpected input.

## Test Approach

The tests were performed **manually** to simulate real-user behavior on the **OrangeHRM Login page**. The tests were conducted across different browsers and devices to ensure **cross-browser compatibility** and **mobile responsiveness**.

### Key Testing Areas:
- **Functional Testing**: Verify valid and invalid login scenarios.
- **Security Testing**: Validate the login page against **SQL injection**.
- **Usability Testing**: Ensure proper field validations and error messages.
- **UI Testing**: Check for proper password masking and field alignment.
  
Test results are logged, and issues are reported to track the progress of the testing phase.

## Test Cases

### Positive Test Cases:
1. **Valid Login**:  
   Test that the user can log in with correct username and password.

2. **Password Masking**:  
   Ensure that the password is properly masked (asterisks or dots) when entered into the password field.

### Negative Test Cases:
1. **Invalid Login - Incorrect Username**:  
   Test login with an incorrect username and correct password.

2. **Invalid Login - Incorrect Password**:  
   Test login with a correct username but incorrect password.

3. **Empty Username Field**:  
   Test login with the username field empty.

4. **Empty Password Field**:  
   Test login with the password field empty.

5. **SQL Injection**:  
   Test for **SQL injection vulnerabilities** by entering malicious code in the username or password field.

## Test Execution

The tests were executed manually across multiple browsers (Chrome, Firefox, Safari) and devices (Desktop, Mobile). Below is an execution log for each of the test cases:

| **Test Case ID** | **Test Case Description**                             | **Execution Date**  | **Status**  | **Remarks**             |
|------------------|-------------------------------------------------------|---------------------|-------------|-------------------------|
| TC01             | Valid Login: Login with correct username and password | January 15, 2025    | Passed      | Successful login        |
| TC02             | Password Masking: Ensure password is masked          | January 15, 2025    | Passed      | Password masked correctly|
| TC03             | Invalid Login - Incorrect Username                   | January 16, 2025    | Passed      | Error message displayed |
| TC04             | Invalid Login - Incorrect Password                   | January 16, 2025    | Passed      | Error message displayed |
| TC05             | Empty Username Field                                 | January 17, 2025    | Passed      | Validation message shown|
| TC06             | Empty Password Field                                 | January 17, 2025    | Passed      | Validation message shown|
| TC07             | SQL Injection Test                                   | January 18, 2025    | Passed      | Login failed as expected|

---

## Bug Reports

A **bug report** has been created for the issue where the login form does not show an error message when the **username field** is left empty. This is a **high severity** bug that needs to be addressed by the development team.

### Bug Report Sample:

**Bug Report**  
**Version**: 1.0  
**Date**: January , 2025  
**Prepared by**: Varshitha B

---

## Test Summary Report

### **Summary**  
This report summarizes the testing activities for the **OrangeHRM Login** feature. All test cases were executed successfully with no critical issues found, except for a minor bug related to the empty username field. The system was tested for both functional and security aspects, including **SQL injection**.

### **Total Test Cases**: 7  
- **Passed**: 7  
- **Failed**: 0  
- **Blocked**: 0  

### **Conclusion**  
The **OrangeHRM Login functionality** is working as expected, with all positive and negative test scenarios passing successfully. The system is secure against **SQL injection** attacks and handles invalid inputs correctly. However, there is a bug in the validation of the username field when it is left empty.

---

## How to Run Tests

To replicate or extend the tests in this repository:

1. **Clone this repository** to your local machine:
```bash
   git clone https://github.com/CV0412/Manual-Testing-OrangeHRM_Login.git
```
## Set up your testing environment:

Use a web browser like Google Chrome, Firefox, or Safari to open the login page.
Test manually by following the test cases listed in the Test Cases section above.

**Record your results:**
Document the outcomes of each test case in the Test Execution Log.
If any issues arise, follow the Bug Report Template to log and track them.

## Technologies Used
**Manual Testing:** For testing the login functionality on the web.
**Browsers:** Chrome, Firefox, Safari
**Tools:** Excel (for Test Cases and Execution Logs), Word (for Bug Reports and Summary)
**Web:** https://opensource-demo.orangehrmlive.com/web/index.php/auth/login for testing

Feel free to contribute to this repository by suggesting more test cases, improving the documentation, or helping with bug fixes. Happy testing!

