# saucedemo_cases – Manual Test Cases

This project contains manual test cases written for [SauceDemo](https://www.saucedemo.com/), an e-commerce demo website. The purpose of this project is to practice manual testing across key user flows like login, cart management, and checkout.

## Application Under Test
Website      : https://www.saucedemo.com/
Type         : E-commerce demo application
Credentials  : Username: standard_user / Password: secret_sauce

## Testing Type
1. Manual Testing
2. Functional Testing
3. Negative Testing
4. Boundary / Edge Case Testing

## Test Case Structure
Each test case includes the following fields:
1. SR No. – Serial number
2. Test Scenario ID – Unique ID for the scenario
3. Module – Feature being tested
4. Test Scenario Description – High-level description of what is being tested
5. Test Case ID – Unique ID for each test case
6. Test Case Description – Detailed description of the test
7. Test Steps – Step-by-step instructions to execute the test
8. Test Data – Input data used during testing
9. Expected Result – What should happen
10. Actual Result – What actually happened during testing
11. Status – Pass / Fail

## Bugs Found
### TC_001_02 – Login fails with uppercase username
Description: Application does not accept uppercase username (e.g. `STANDARD_USER`), showing an error even though it is the correct username.
Expected: Login should succeed (case-insensitive).
Actual: Error message — "Username and password do not match any user in this service."
![TC_001_02 Screenshot](screenshots/TC_001_02_uppercase_login_fail.png)

### TC_003_06 – Special characters accepted in name fields at checkout
Description: Entering special characters (e.g. `nikk@12`) in the First Name field during checkout does not show any validation error. The checkout process continues as normal.
Expected: An error message should appear for invalid characters.
Actual: No error shown — checkout continues.
![TC_003_06 Screenshot](screenshots/TC_003_06_special_chars_fail.png)

### TC_003_07 – Numeric values accepted in name fields at checkout
Description: Entering numbers (e.g. `12234544`) in the First Name field does not trigger any validation. The form accepts it and proceeds.
Expected: An error message should appear for invalid numeric input.
Actual: No error shown — checkout continues.
![TC_003_07 Screenshot](screenshots/TC_003_07_numeric_name_fail.png)

### TC_003_09 – Zip code field accepts alphabetic characters
Description: The postal/zip code field should only accept numeric values, but entering alphabetic characters does not trigger any error and the checkout continues.
Expected: Error message shown for non-numeric zip code input.
Actual: No validation — checkout continues without error.
![TC_003_09 Screenshot](screenshots/TC_003_09_zipcode_chars_fail.png)

## Test Coverage
I have tested modules Login, Product Add to Cart, and Checkout with test scenario IDs TC_001, TC_002, and TC_003 respectively. I have designed and executed a total of 26 test cases across all three modules — Login has 9, Product Add to Cart has 8, and Checkout has 9 test cases respectively.

## Tools Used
1. Microsoft Excel (test case documentation)
2. Browser: Chrome, Firefox (cross-browser testing)

## Author
Nikita Dhopte
QA Tester
GitHub: https://github.com/nikitad-QA






