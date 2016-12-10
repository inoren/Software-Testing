# Testplan

## 1. Introduction
### 1.1 Purpose

### 1.2 Background

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

### 1.5 References
All references are in the subfolder "References".

1. [WebServer_Requirements_v1.0][1]
2. Scenario_paper_v1.0

## 2. Requirements for Test
The listing below (uses cases, functional-requirements and non-functional-requirements) identifies all items that have been identified as targets for testing. It represents what will be tested.

### 2.1 Data and Database Integrity Testing

- Requirements Document, Use Case 3: "System delivers the shared resource to the browser[[1]]"
- Verify access to shared resource folder
- Verify correct retrieval of data from the shared resource folder
- Verify simultaneous record read accesses.

### 2.2  Unit Testing
- None

### 2.3 Function Testing
- Requirements Document, Supplementary Specification Req 3.: "The web server must work on Linux, Mac, Windows(XP, Vista, 7,8,10,Server 2008)[[1]]"
- Scenario paper: "easy integration and adaptation of the web-server[[2]]"
- Requirements Document, Supplementary Specification Req 2.: "The web server must follow minimum requirements for HTTP 1.1[[1]]"
- Requirements Document, Supplementary Specification Req 5.: "Req 5. The access log should be viewable from a text editor.[[1]]"

### 2.4 Business Cycle Testing
- Requirements Document, Supplementary Specification Req 4.: "The source code should be released under GPL-2.0.[[1]]"

### 2.5 User Interface Testing
- Verify easy access for customer. ([Scenario paper][2])
- Verify ease of navigation through a sample set of screens.

### 2.6 Performance Testing
- None

### 2.7 Load Testing
-  Requirements Document, Supplementary Specification Req 1.: "The web server should be responsive under high load.[[1]]"

### 2.8 Stress Testing
None

### 2.9 Security & Access Testing
- The web-server should provide absolute security.([Scenario paper][2])

### 2.10 Recovery Testing
None

### 2.11 Configuration Testing
- The web-server should need minimal configuration.([Scenario paper][2])

### 2.12 Installation Testing
- The web-server should be easy to deploy.

### 2.13 Acceptance Testing
None



[1]: https://github.com/onkelhoy/Software-Testing/blob/master/Assignment%202/References/WebServer_Requirements_v1.0.pdf
[2]: https://github.com/onkelhoy/Software-Testing/blob/master/Assignment%202/References/Scenario_paper_v1.0.pdf
