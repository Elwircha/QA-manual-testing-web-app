# Test Plan for Login Form Testing

## 1. Introduction
### Objective of Testing:
To verify the functionality, validation, and security of the login form on the website. Ensure the form operates correctly for all scenarios, including successful login, error handling, and protection against invalid actions.

### Test Object:
Login page of [The Internet](https://the-internet.herokuapp.com/login)

### Test Items:
Verification of the login page display
Validation of username/password correctness
Behavior testing with invalid data input
Error message testing

## 2. Scope and Boundaries
### Features to Be Tested:
Correct functionality of the "Username" and "Password" fields
Validation of the "Login" button
Error messages for invalid data
User redirection after successful login
UI/UX testing (ease of use, element display)

### Features Not to Be Tested:
Website performance
API testing

## 3. Approach
### Testing Types:

**Functional Testing:**
Validate the core functionalities of the form.

**UI/UX Testing:**
Assess the display of form elements and their usability.

**Negative Testing:**
Test the system's behavior when incorrect data is entered.

**Security Testing:**
Attempt SQL injection and XSS attacks.

**Tools:**
Manual testing for user scenarios.
Automation: Selenium for automating test cases

## 4. Expected Risks
Potential failures when attempting attacks such as SQL injection
Incorrect error messages
Insufficient client-side validation

## 5. Test Deliverables
Defect report (via Jira)
Screenshots and error logs
Recommendations for improvement if issues are identified

## 6. Metrics Used
Percentage of test cases passed
Number of defects found

## 7. Conclusion
This test plan will facilitate an effective evaluation of the login form's functionality.