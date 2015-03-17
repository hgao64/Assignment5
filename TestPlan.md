# Test Plan

Test strategy and test cases were planed in this document below. The test strategy describes the approaches to test the software in its development cycle. The test cases describes the purpose, steps, results and other related information. 

**Author**: Huihui Duan

## 1 Testing Strategy

### 1.1 Overall strategy

In the unit test, input validation test will be performed by Huihui Duan and Hui Gao; in the integration test and system test, lifecycle event, runtime configuration changes and screen sizes and resolutions tests will be performed by Huihui Duan and Hui Gao. Regression testing will also be needed if there are some changes made for enhancement. 

### 1.2 Test Selection

Both of black-box and white-box techniques will be used to test in unit level, integration level, and system level. 

### 1.3 Adequacy Criterion

**Functional Coverage**

Customer input validation, Discount validation, purchase input and reading validation functionality coverages should be tested in the test cases. 

**Structural Coverage**

The test cases should cover the components and interconnect to perform customer input, transaction, purchase summary, and discount applying etc. 


### 1.4 Bug Tracking

A database will be created to record the known bugs. The database include the time a bug was report, the severity, detailed analysis of the bug, the person who is working on fixing the bug, and also the progress of the fix. 

### 1.5 Technology

JUnit test classes will be implemented to test all methods. 

## 2 Test Cases

For each test case below, it provides purpose, the steps necessary to perform the test, the expected result, the actual result (to be filled later), pass/fail information (to be filled later), and any additional information which is relevant. JUnit test cases need to be updated. 

| Test Case # | Purpose       | Steps         | Expected Result  |   Actual Result  | Pass/Fail Info | Other Info |
| ----------- | ------------- |:-------------:| :-------------:  |:-------------:   |:-------------: | ---------- |
| 1 | Customer Input | First Name: Huihui; Last Name： Duan; Zip Code: 91406; Email: hduan30@gatech.edu |  |  |  |  |
| 2 | Customer Input | First Name: 123; Last Name： Duan; Zip Code: 91406; Email: hduan30@gatech.edu |  |  |  |  |
| 3 | Customer Input | First Name: Huihui; Last Name： 456; Zip Code: 91406; Email: hduan30@gatech.edu |  |  |  |  |
| 4 | Customer Input | First Name: Huihui; Last Name： Duan; Zip Code: ABCDE; Email: hduan30@gatech.edu |  |  |  |  |
| 5 | Customer Input | First Name: Huihui; Last Name： Duan; Zip Code: 91406; Email: hduan30#gatech.edu |  |  |  |  |
| 6 | Purchase Input | Date: Mar-3-15; Amount: $157 |  |  |  |  |
| 7 | Purchase Input | Date: 12345678; Amount: $157 |  |  |  |  |
| 8 | Purchase Input | Date: Mar-3-15; Amount: ABCD |  |  |  |  |
