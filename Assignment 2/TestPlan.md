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

## 2. Requirements for Test
The listing below (uses cases, functional-requirements and non-functional-requirements) identifies all items that have been identified as targets for testing. It represents what will be tested.

### 2.1 Data and Database Integrity Testing

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

### 2.7 Load Testing
-  Requirements Document, Supplementary Specification Req 1.: "The web server should be responsive under high load.[[1]]"

### 2.8 Stress Testing
- Verify web-server response when accessing it from various IoT-Devices in a LAN.

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


[1]: https://github.com/onkelhoy/Software-Testing/blob/master/Assignment%202/References/WebServer_Requirements_v1.0.pdf
[2]: https://github.com/onkelhoy/Software-Testing/blob/master/Assignment%202/References/Scenario_paper_v1.0.pdf
