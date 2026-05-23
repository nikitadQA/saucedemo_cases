# saucedemo_cases :- Manual test cases

This project contains manual test cases written for [Burst Oralcare](https://burstoralcare.com/), a real-world oral care e-commerce website. The purpose of this project is to practice manual testing on a live production website, covering sign-up functionality and product search.

Application Under Test :
Field Details Website :- https://www.saucedemo.com/
Type E-commerce demo application Test 
credentials Username : standard_user / Password: secret_sauce

Testing Type :
1. Manual Testing
2. Functional Testing
3. Negative Testing
4. Boundary / Edge Case Testing

Test Coverage :
Module                        Test Scenario ID     No. of Test Cases   
Login                                TC_001                 9
Product Add to Cart                  TC_002                 8
Checkout                             TC_003                 9
Total                                                       26

Test Case Structure :
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

Bugs Found :
1. TC_001_02 – Login fails with uppercase username
Description:Application does not accept uppercase username (e.g. `STANDARD_USER`), showing an error even though it is the correct username.  
Expected:Login should succeed (case-insensitive).  
Actual:Error message — "Username and password do not match any user in this service."

![TC_001_02 Screenshot](screenshots/TC_001_02_uppercase_login_fail.png)

Tools Used :
1. Microsoft Excel(test case documentation)
2. Browser: Chrome, Firefox(cross-browser testing)

Author :
Nikita Dhopte
QA Tester
GitHub: nikitad-QA









