# SauceDemo – Manual Test Cases
This project contains manual test cases written for the [SauceDemo](https://www.saucedemo.com/) e-commerce demo website. The purpose of this project
is to practice real-world manual testing across key user flows like login, cart management, and checkout.

Application Under Test :
Website : https://www.saucedemo.com/ 
Type : E-commerce demo application 
Test credentials : Username: `standard_user`  Password: `secret_sauce` 

 Test Coverage: 
 I have tested module login, product add to cart and checkcout which have id TC_001, TC_002, TC_003. Total 26 number of test cases i have design and executed
 for all three modules with positive and negative scenario. For login have 9, for add product to cart have 8 and for checkout have 9 test cases.

 Test Case Structure :
 Each test case includes the following fields:
- SR No. : Serial number
- Test Scenario ID : Unique ID for the scenario
- Module : Feature being tested
- Test Scenario Description : High-level description of what is being tested
- Test Case ID : Unique ID for each test case
- Test Case Description : Detailed description of the test
- Test Steps : Step-by-step instructions to execute the test
- Test Data : Input data used during testing
- Expected Result : What should happen
- Actual Result : What actually happened during testing
- Status : Pass / Fail

 Bugs Found :

1. TC_001_02 – Login fails with uppercase username
Description:Application does not accept uppercase username (e.g. `STANDARD_USER`), showing an error even though it is the correct username.  
Expected:Login should succeed (case-insensitive).  
Actual:Error message — "Username and password do not match any user in this service."
![TC_001_02 Screenshot](screenshots/TC_001_02_uppercase_login_fail.png)

2. TC_003_06 – Special characters accepted in name fields at checkout

Description:Entering special characters (e.g. `nikk@12`) in the First Name field during checkout does not show any validation error. The checkout process continues as normal.  
Expected:An error message should appear for invalid characters.  
Actual:No error shown — checkout continues.
![TC_003_06 Screenshot](screenshots/TC_003_06_special_chars_fail.png)

---

3. TC_003_07 – Numeric values accepted in name fields at checkout

Description:Entering numbers (e.g. `12234544`) in the First Name field does not trigger any validation. The form accepts it and proceeds.  
Expected:An error message should appear for invalid numeric input.  
Actual:No error shown — checkout continues.
![TC_003_07 Screenshot](screenshots/TC_003_07_numeric_name_fail.png)

4. TC_003_09 – Zip code field accepts alphabetic characters
Description:The postal/zip code field should only accept numeric values, but entering alphabetic characters does not trigger any error and the checkout continues.
Expected:Error message shown for non-numeric zip code input.  
Actual:No validation — checkout continues without error.
![TC_003_09 Screenshot](screenshots/TC_003_09_zipcode_chars_fail.png)

Testing Type :
- Manual Testing
- Functional Testing
- Negative Testing
- Boundary / Edge Case Testing

Tools Used :
- Microsoft Excel (test case documentation)
- Browser: Chrome, Firefox (cross-browser testing)

 
QA Tester  
GitHub: [nikitad-QA](https://github.com/nikitad-QA)
