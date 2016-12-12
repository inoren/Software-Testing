# Testplan

## 1. Introduction
### 1.1 Purpose
The purpose of this test plan document is to support the followings objectives:
- Evaluate the current state and find possible risks in the given open source project
- Illustrates the recommended requirements for test
- Explain and recommend the testing strategies
- Classify the appropriate resources and bring an evaluation of the test achievements
- List the result of test project  

### 1.2 Background
My Web Server is an open source software. The Software Development Company (SDC) plans to use this server on large-scale of Internet of Things (IOT) in order to display the information from sensors. SDC wants to evaluate whether this server fulfills all of their security, functional and performance needs.  

### 1.4 Goals
- SDC
 - easy deploy
 - wide range: many deployable devices
- Developer
 - minimal configuration
 - easy integration: unambiguous API
- Customer
 - easy access
 - absolute security

### 1.3 Scope
This test plan applies to Data and Database Integrity Testing, Unit Testing, Function Testing, Business Cycle Testing, User Interface Testing, Performance Testing, Load Testing, Stress Testing, Security & Access Testing, API Testing, Configuration Testing and Installation Testing. All these tests will be conducted in this iteration. Information regarding the aim of these tests can be find in Section 2 (Requirements for Test).

### 1.5 References
All references are in the subfolder "References".

1. [WebServer_Requirements_v1.0][1]
2. [Scenario_paper_v1.0] [2]

[1]: https://github.com/onkelhoy/Software-Testing/blob/master/Assignment%202/References/WebServer_Requirements_v1.0.pdf
[2]: https://github.com/onkelhoy/Software-Testing/blob/master/Assignment%202/References/Scenario_paper_v1.0.pdf

## 2. Requirements for Test
The listing below (uses cases, functional-requirements and non-functional-requirements) identifies all items that have been identified as targets for testing. It represents what will be tested.

### 2.1 Data Integrity Testing

- Requirements Document, Use Case 3: "System delivers the shared resource to the browser[[1]]"
- Verify access to shared resource folder
- Verify correct retrieval of data from the shared resource folder
- Verify simultaneous record read accesses.

### 2.2  Unit Testing
- Confirm proper functioning of Unit-Tests from existing JUnit-Testsuit.
- Verify coverage of units by existing unit-tests.

### 2.3 Function Testing
- Requirements Document, Supplementary Specification Req 3.: "The web server must work on Linux, Mac, Windows(XP, Vista, 7,8,10,Server 2008)[[1]]"
- Requirements Document, Supplementary Specification Req 2.: "The web server must follow minimum requirements for HTTP 1.1[[1]]"
- Requirements Document, Supplementary Specification Req 5.: "Req 5. The access log should be viewable from a text editor.[[1]]"
- Verify start correct start of the web-server.
- Verify normal termination of web-server.
- Verify correctness of existing automated integration-, response- and log- tests.
- Verify correct working of the web-server in a local-network.

### 2.4 Business Cycle Testing
- Requirements Document, Supplementary Specification Req 4.: "The source code should be released under GPL-2.0.[[1]]"

### 2.5 User Interface Testing
- Verify easy access for customer. ([Scenario paper][2])

### 2.6 Performance Testing
- Verify start of web-server in a reasonable time.
- Performance Profiling of responses from web-server deployed in different OS-environments.
- Verify web-server response when accessing it from various IoT-Devices in a LAN.

### 2.7 Load Testing
-  Requirements Document, Supplementary Specification Req 1.: "The web server should be responsive under high load.[[1]]"

### 2.8 Stress Testing
- None

### 2.9 Security & Access Testing
- The web-server should provide absolute security.([Scenario paper][2])

### 2.10 Recovery Testing
- None

### 2.11 API Testing
- Scenario paper: "easy integration and adaptation of the web-server[[2]]"

### 2.12 Configuration Testing
- The web-server should need minimal configuration.([Scenario paper][2])

### 2.13 Installation Testing
- The web-server should be easy to deploy.

### 2.14 Acceptance Testing
- None

## 3. Test Strategy
The Test Strategy presents a recommended approach of testing the identified testing-targets. The previous section described *what* are the testing-targets.
This section will describe *how* it will be tested.The main considerations for the test strategy are the techniques to be used and the criterion for knowing when the testing is completed.

### 3.1 Testing-types

#### 3.1.1 Data Integrity Testing
The data access and process should be tested within the running system. The retrieval of data can be tested in an automated suite, while the integrity and correctness must be tested manually.

![Data_Integrity_Testing](https://github.com/onkelhoy/Software-Testing/blob/master/Assignment%202/Resources/Test_Strategies_Tables/DataIntegrityTesting.png "Inline style")

#### 3.1.2 Unit Testing
![Unit_Testing](https://github.com/onkelhoy/Software-Testing/blob/master/Assignment%202/Resources/Test_Strategies_Tables/UnitTesting.png "Inline style")

#### 3.1.3 Function Testing
The testing of the application should focus on any target requirements that can be traced directly from the use-cases or the Scenario-goals. This type of testing is based up on black-box-testing, while testing the completeness of the existing tests is done with code-coverage and white-box testing.

![Function_Testing](https://github.com/onkelhoy/Software-Testing/blob/master/Assignment%202/Resources/Test_Strategies_Tables/FunctionTesting.png "Inline style")

#### 3.1.4 Business Cycle Testing
This section is not applicable to test because it is a legal-matter.
Redirected to legal department.

#### 3.1.5 User Interface Testing
![User_Interface_Testing](https://github.com/onkelhoy/Software-Testing/blob/master/Assignment%202/Resources/Test_Strategies_Tables/UserInterfaceTesting.png "Inline style")

#### 3.1.6 Performance Testing
![Performance_Testing](https://github.com/onkelhoy/Software-Testing/blob/master/Assignment%202/Resources/Test_Strategies_Tables/PerformanceTesting.png "Inline style")

#### 3.1.7 Load Testing
![Load_Testing](https://github.com/onkelhoy/Software-Testing/blob/master/Assignment%202/Resources/Test_Strategies_Tables/LoadTesting.png "Inline style")

#### 3.1.8 Stress Testing
None

#### 3.1.9 Security & Access Testing
The testing will depend on an external tool which should be up-to-date with the current standards and verifies a proper level of security for known vulnerabilities.

![Security_Testing](https://github.com/onkelhoy/Software-Testing/blob/master/Assignment%202/Resources/Test_Strategies_Tables/SecurityTesting.png "Inline style")

#### 3.1.10 Recovery Testing
None

#### 3.1.11 API Testing
This section is not applicable to test because no API is provided.

#### 3.1.12 Configuration Testing
![Configuration_Testing](https://github.com/onkelhoy/Software-Testing/blob/master/Assignment%202/Resources/Test_Strategies_Tables/ConfigurationTesting.png "Inline style")

#### 3.1.13 Installation Testing
![Installation_Testing](https://github.com/onkelhoy/Software-Testing/blob/master/Assignment%202/Resources/Test_Strategies_Tables/InstallationTesting.png "Inline style")

#### 3.1.14 Acceptance Testing
None

### 3.2 Tools
The following tools will be employed for testing:
![Tools_Table](https://github.com/onkelhoy/Software-Testing/blob/master/Assignment%202/Resources/Test_Strategies_Tables/ToolsTable.png "Inline style")

## 4. Resources
The resources for the MyWebServer test effort are the SDC-employees of the testing-team.

### 4.1 Workers
![Resources_Workers_Table](https://github.com/onkelhoy/Software-Testing/blob/master/Assignment%202/Resources/ResourcesWorkersTable.png "Inline style")


### 4.2 System
The server module will mainly run on the defined PC's as localhost. For some function tests it will be emulated on VM's. The access tests will be done from various client systems to ensure compatibility and meet the requirements. Whole test-suits will just run on the listed PC-OS's.

![Resources_System_Table](https://github.com/onkelhoy/Software-Testing/blob/master/Assignment%202/Resources/SystemResourcesTable.png "Inline style")

The server test stations must have the following software installed and properly configured:

- JAVA 8 JDK

The server needs to be setup locally or remotely to run each test suit.
The default configuration used:
- port: 1091
- shared resource folder: /MyWebServer/tests/se/lnu/http/resources/inner

## 5. Project Milestones
The dates are just estimates and may vary since iteration-efforts may depend on each other. So planning and working will be done in an agile-way as defined in the test-plan.

![Project_Milestones_Table](https://github.com/onkelhoy/Software-Testing/blob/master/Assignment%202/Resources/ProjectMilestonesTable.png "Inline style")

## 6. Deliverables

### 6.1 Test Plan
The Test Plan will define *who* does *what* in which iteration. It divides the test-effort into manageable iterations and sets time-limitations.

### 6.2 Test Model
The Test Model will define all the test cases and will reference the test procedures, tools and test-scripts which are associated with each test-case.

### 6.3 Test Results
For each test executed a test-result form will be created. This should include the name or ID of the test-case or specification it relates to, the execution-date, name of the tester and the result of the test.

### 6.4 Test Report
A final evaluation of the test-activities and their results will be presented.
