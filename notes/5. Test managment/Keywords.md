# 5 Test Management (225 minutes)

### Keywords
- **Configuration management**
- **Defect management**
- **Defect report**
- **Entry criteria**
- **Exit criteria**
- **Product risk**
- **Project risk**
- **Risk**
- **Risk level**
- **Risk-based testing**
- **Test approach**
- **Test control**
- **Test estimation**
- **Test manager**
- **Test monitoring**
- **Test plan**
- **Test planning**
- **Test progress report**
- **Test strategy**
- **Test summary report**
- **Tester**

---

## Learning Objectives for Test Management

### 5.1 Test Organization
- **FL-5.1.1 (K2):** Explain the benefits and drawbacks of independent testing.
- **FL-5.1.2 (K1):** Identify the tasks of a test manager and tester.

### 5.2 Test Planning and Estimation
- **FL-5.2.1 (K2):** Summarize the purpose and content of a test plan.
- **FL-5.2.2 (K2):** Differentiate between various test strategies.
- **FL-5.2.3 (K2):** Give examples of potential entry and exit criteria.
- **FL-5.2.4 (K3):** Apply knowledge of prioritization and technical/logical dependencies to schedule test execution for a given set of test cases.
- **FL-5.2.5 (K1):** Identify factors that influence the effort related to testing.
- **FL-5.2.6 (K2):** Explain the difference between two estimation techniques: metrics-based and expert-based techniques.

### 5.3 Test Monitoring and Control
- **FL-5.3.1 (K1):** Recall metrics used for testing.
- **FL-5.3.2 (K2):** Summarize the purposes, contents, and audiences for test reports.

### 5.4 Configuration Management
- **FL-5.4.1 (K2):** Summarize how configuration management supports testing.

### 5.5 Risks and Testing
- **FL-5.5.1 (K1):** Define risk level using likelihood and impact.
- **FL-5.5.2 (K2):** Distinguish between project and product risks.
- **FL-5.5.3 (K2):** Describe how product risk analysis may influence the thoroughness and scope of testing, using examples.

### 5.6 Defect Management
- **FL-5.6.1 (K3):** Write a defect report covering a defect found during testing.


5.1 Test Organization
5.1.1 Independent Testing
Testing tasks may be done by people in a specific testing role, or by people in another role (e.g., customers). A certain degree of independence often makes the tester more effective at finding defects due to differences between the author’s and the tester’s cognitive biases (see section 1.5). Independence is not, however, a replacement for familiarity, and developers can efficiently find many defects in their own code.
Degrees of independence in testing include the following (from low level of independence to high level):
• No independent testers; the only form of testing available is developers testing their own code
• Independent developers or testers within the development teams or the project team; this could be developers testing their colleagues’ products
• Independent test team or group within the organization, reporting to project management or executive management
• Independent testers from the business organization or user community, or with specializations in specific test types such as usability, security, performance, regulatory/compliance, or portability
• Independent testers external to the organization, either working on-site (in-house) or off-site (outsourcing)
For most types of projects, it is usually best to have multiple test levels, with some of these levels handled by independent testers. Developers should participate in testing, especially at the lower levels, so as to exercise control over the quality of their own work.
The way in which independence of testing is implemented varies depending on the software development lifecycle model. For example, in Agile development, testers may be part of a development team. In some organizations using Agile methods, these testers may be considered part of a larger independent test team as well. In addition, in such organizations, product owners may perform acceptance testing to validate user stories at the end of each iteration.
Potential benefits of test independence include:
• Independent testers are likely to recognize different kinds of failures compared to developers because of their different backgrounds, technical perspectives, and biases
• An independent tester can verify, challenge, or disprove assumptions made by stakeholders during specification and implementation of the system
• Independent testers of a vendor can report in an upright and objective manner about the system under test without (political) pressure of the company that hired them
Potential drawbacks of test independence include:
• Isolation from the development team, may lead to a lack of collaboration, delays in providing feedback to the development team, or an adversarial relationship with the development team
• Developers may lose a sense of responsibility for quality
• Independent testers may be seen as a bottleneck
• Independent testers may lack some important information (e.g., about the test object)
