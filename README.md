# 🏨 Adactin Hotel Booking – Manual Testing Project

## 📌 Project Overview

This project demonstrates end-to-end manual testing of the **Adactin Hotel Booking Application**.

The objective of the project is to verify the functionality of the hotel booking application by designing test scenarios, creating test cases, executing test cases, identifying defects, documenting defects, and performing retesting/regression testing activities.

The testing process was carried out based on the available Software Requirements Specification (SRS) and application functionality.

---

# 🎯 Project Objective

The main objectives of this project are:

- Understand the application requirements.
- Identify application modules and testable functionality.
- Design positive and negative test scenarios.
- Create detailed test cases.
- Execute test cases against the application.
- Validate expected and actual results.
- Identify and document defects.
- Assign appropriate severity and priority.
- Perform defect retesting after fixes.
- Perform regression testing for impacted functionality.
- Maintain testing documentation.
- Demonstrate an end-to-end QA testing workflow.

---

# 🏨 Application Overview

The Adactin application is a hotel booking application that allows users to:

- Register as a new user.
- Login using valid credentials.
- Search for hotels based on required criteria.
- Select a hotel.
- Enter booking and personal details.
- Complete hotel booking.
- Generate an order/booking ID.
- View booked itinerary details.
- Search for an existing booking.
- Cancel a booking where applicable.
- Logout from the application.

---

# 📋 Requirements Scope

The application requirements cover the following major areas:

1. New User Registration
2. Login
3. Search Hotel
4. Select Hotel
5. Book Hotel
6. Order Generation
7. Booked Itinerary
8. Cancel Booking
9. Logout

The requirements include both functional behavior and validation requirements for the application.

---

# 🧩 Application Modules

## 1. New User Registration

Tested functionalities include:

- Registration page navigation
- Required field validation
- Username validation
- Password validation
- Confirm password validation
- Full name validation
- Email validation
- CAPTCHA validation
- Terms and Conditions validation
- CAPTCHA refresh
- Reset functionality
- Terms and Conditions link
- Navigation back to Login

### Example validations

- Blank mandatory fields
- Username length validation
- Password length validation
- Password and Confirm Password mismatch
- Invalid email format
- Invalid CAPTCHA
- Terms and Conditions checkbox
- Boundary and negative input validation

---

## 2. Login

Tested functionalities include:

- Valid username and password
- Invalid username
- Invalid password
- Invalid username and password
- Blank username
- Blank password
- Blank username and password
- Login button functionality
- Error message validation
- Successful navigation to Search Hotel page

---

## 3. Search Hotel

Tested functionalities include:

- Hotel location
- Hotel selection
- Room type
- Number of rooms
- Check-in date
- Check-out date
- Adults per room
- Children per room
- Search button
- Mandatory field validations
- Invalid input validations
- Search result validation

---

## 4. Select Hotel

Tested functionalities include:

- Display of available hotels
- Hotel selection
- Select Hotel functionality
- Continue button
- Navigation to Book Hotel page

---

## 5. Book Hotel

Tested functionalities include:

- First Name
- Last Name
- Billing Address
- Credit Card Number
- Credit Card Type
- Expiry Month
- Expiry Year
- CVV
- Book Now functionality
- Cancel functionality
- Input field validations
- Boundary value validations
- Invalid character validations

---

## 6. Order Generation

Tested functionalities include:

- Successful hotel booking
- Order number generation
- Order number display
- Booking confirmation
- Order number retrieval

---

## 7. Booked Itinerary

Tested functionalities include:

- Navigate to Booked Itinerary
- Search using Order ID
- Go/Search functionality
- Order ID validation
- Booking information display
- Invalid Order ID handling

---

## 8. Cancel Booking

Tested functionality includes:

- Selecting an existing booking
- Cancelling the booking
- Booking cancellation confirmation
- Validation of cancelled booking

---

## 9. Logout

Tested functionality includes:

- Logout link/button
- Session termination
- Navigation after logout
- Access restriction after logout where applicable

---

# 🧪 Testing Types

The following testing approaches were considered during the project:

### Functional Testing

To verify that each application function works according to the expected requirement.

### UI Testing

To verify UI elements such as:

- Buttons
- Text fields
- Dropdowns
- Links
- Checkboxes
- Messages
- Navigation

### Positive Testing

Testing the application using valid inputs and valid user flows.

### Negative Testing

Testing the application using invalid, incomplete, blank, boundary, and unexpected inputs.

### Boundary Value Testing

Testing values around defined limits.

Examples:

- Minimum value
- Minimum - 1
- Maximum value
- Maximum + 1

### Validation Testing

Validating field-level restrictions and error messages.

### Integration Testing

Validating the flow between related modules.

Example:

Login → Search Hotel → Select Hotel → Book Hotel → Order Generation

### End-to-End Testing

Validating the complete business flow from login through hotel booking and order generation.

### Retesting

Re-executing failed test cases after defects are fixed.

### Regression Testing

Verifying that changes or fixes do not negatively affect existing functionality.

---

# 📝 Test Scenario Design

Test scenarios were derived from the application requirements and modules.

The scenarios cover:

- Valid conditions
- Invalid conditions
- Mandatory fields
- Boundary conditions
- Field validations
- Navigation
- Business workflow
- Error handling

Each scenario is mapped to corresponding test cases using a Test Scenario ID.

---

# 🧾 Test Case Design

The test case document contains detailed test cases with:

- Test Case ID
- Test Scenario ID
- Test Steps
- Input Data
- Expected Result
- Actual Result
- Pass/Fail status
- Comments
- Defect ID where applicable

### Test Case Example

| Test Case | Scenario | Description | Expected Result |
|---|---|---|---|
| TC_001 | TS_001 | Login with valid credentials | User should login successfully |
| TC_002 | TS_001 | Login with invalid username | Invalid username message should appear |
| TC_003 | TS_001 | Login with invalid password | Invalid password message should appear |
| TC_004 | TS_001 | Login with invalid username and password | Appropriate error message should appear |

---

# 📊 Test Execution

A total of **147 test cases** are documented in the current test-case workbook.

Test execution results are recorded against individual test cases using:

- Pass
- Fail
- Not Executable
- Comments
- Defect ID

The execution sheet also records actual results against expected results.

---

# 🐞 Defect Management

Defects identified during testing were documented using a structured defect template.

The defect report contains fields such as:

- Defect ID
- Status
- Severity
- Priority
- Module
- Reported By
- Browser
- Found in Version
- Found in Build
- Fixed in Version
- Fixed in Build
- Defect Title
- Description
- Steps to Reproduce
- Expected Result
- Actual Result

---

# 🐛 Defects Identified

The defect documentation contains defects ranging from:

- BUG001
- BUG002
- ...
- BUG026

The defects cover issues identified in modules such as:

- New User Registration
- Search Hotel
- Book Hotel
- Book Itinerary

Examples of validation issues identified include:

- Invalid characters accepted in input fields
- Invalid numeric values accepted
- Invalid special characters accepted
- Invalid billing address input accepted
- Invalid credit card number input accepted
- Invalid CVV input accepted
- Past expiry year accepted
- Book Itinerary search/Go functionality issues
- Invalid Order ID input handling issues

---

# 🔍 Example Defect

### Defect ID

`BUG012`

### Module

`Book Hotel`

### Title

`Billing Address is accepting number only in Book Hotel Page`

### Steps to Reproduce

1. Launch the browser.
2. Enter the application URL.
3. Enter valid username.
4. Enter valid password.
5. Click Login.
6. Select the required hotel search criteria.
7. Click Search.
8. Select a hotel.
9. Enter numeric data into the Billing Address field.

### Expected Result

Billing Address should not accept invalid numeric-only input.

### Actual Result

The Billing Address field accepts numeric-only input.

### Browser

Chrome

### Status

New

---

# 🔄 Defect Life Cycle

The defect management process followed in the project can be represented as:

New
 ↓
Assigned
 ↓
Open
 ↓
Fixed
 ↓
Retest
 ↓
Verified
 ↓
Closed
