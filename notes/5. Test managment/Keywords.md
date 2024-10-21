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

### 5.1.2 Tasks of a Test Manager and Tester

In this section, we explore two primary roles in testing: **test managers** and **testers**. The specific tasks and responsibilities for these roles vary depending on project and product context, skill levels, and organizational structure.

#### **Test Manager Tasks**
The **test manager** is responsible for overseeing the entire test process and ensuring the success of the testing activities. This role may be carried out by various individuals such as a test manager, project manager, or quality assurance manager. In larger projects, multiple test teams may report to the test manager, with each team led by a **test leader** or **lead tester**.

Typical tasks of a test manager include:
- **Developing or reviewing test policy and strategy** for the organization.
- **Planning test activities** based on the project context, test objectives, and risks. This includes:
    - Selecting test approaches.
    - Estimating time, effort, and costs.
    - Defining test levels, cycles, and defect management processes.
- **Writing and updating test plans**.
- **Coordinating test plans** with stakeholders such as project managers and product owners.
- **Sharing testing perspectives** with other project teams (e.g., integration planning).
- **Initiating test analysis, design, and execution**, monitoring progress, and checking exit criteria.
- **Preparing test progress and summary reports**.
- **Adapting planning based on test progress and results**.
- **Supporting defect management and configuration management** for testware.
- **Introducing metrics** for test progress and product quality evaluation.
- **Supporting tool selection and implementation** for the test process.
- **Deciding on the implementation of test environments**.
- **Promoting the test team** and the test profession within the organization.
- **Developing testers' skills and careers** (e.g., training plans, coaching).

In **Agile environments**, many of these tasks are handled by the Agile team. Day-to-day testing is often managed by a tester within the team, while tasks that span multiple teams or concern personnel management may still be performed by a test manager or **test coach**.

#### **Tester Tasks**
The **tester** works more hands-on with the testing activities, performing tasks that ensure the quality and functionality of the product. Typical tester tasks include:
- **Reviewing and contributing to test plans**.
- **Analyzing requirements, user stories, acceptance criteria, and specifications** for testability.
- **Identifying and documenting test conditions** and ensuring traceability between test cases and the test basis.
- **Designing, setting up, and verifying test environments**.
- **Designing and implementing test cases and procedures**.
- **Preparing and acquiring test data**.
- **Creating a detailed test execution schedule**.
- **Executing tests, evaluating results**, and documenting deviations.
- **Using tools to support the test process**.
- **Automating tests** as needed, with possible support from developers or automation experts.
- **Evaluating non-functional characteristics** such as performance, reliability, and security.
- **Reviewing tests developed by others**.

Different testers might specialize in certain areas such as **test analysis**, **test design**, or **test automation**. Testers may also vary based on the test level they are involved in:
- **Component and integration testing**: Often handled by developers.
- **Acceptance testing**: Often handled by business analysts, subject matter experts, or users.
- **System and system integration testing**: Usually conducted by independent test teams.
- **Operational acceptance testing**: Typically conducted by operations or systems administration staff.

### 5.2 Test Planning and Estimation

#### 5.2.1 Purpose and Content of a Test Plan
A test plan outlines test activities for both development and maintenance projects. Test planning is influenced by the organization’s test policy, test strategy, development lifecycles, project scope, objectives, risks, constraints, and resource availability. As the project progresses, more information becomes available, and the test plan becomes more detailed. Test planning is a continuous process that spans the product's lifecycle, including maintenance.

Feedback from test activities helps in recognizing changing risks, which allows adjustments in the planning process. A master test plan and separate plans for different test levels (e.g., system testing, acceptance testing) or test types (e.g., usability, performance testing) may be created.

Test planning activities may include:
- Determining the **scope**, **objectives**, and **risks** of testing
- Defining the overall **approach** of testing
- Coordinating the **test activities** with the software lifecycle
- Making decisions about **what to test**, resources required, and how testing will be conducted
- **Scheduling** test activities such as analysis, design, implementation, execution, and evaluation
- Selecting **metrics** for monitoring and control
- **Budgeting** for test activities
- Determining the structure and level of detail for **test documentation**

The content of a test plan may vary depending on the context, but a sample test plan structure can be found in the **ISO standard (ISO/IEC/IEEE 29119-3)**.

#### 5.2.2 Test Strategy and Test Approach
A **test strategy** is a generalized description of the testing process, typically at the product or organizational level. Common types of test strategies include:

- **Analytical**: Based on analysis of a factor such as risk (e.g., risk-based testing).
- **Model-based**: Based on models like business processes, state models, or reliability growth models.
- **Methodical**: Systematic use of predefined tests, such as common failure taxonomies or quality characteristics.
- **Process-compliant**: Based on external rules, standards, or process documentation.
- **Directed**: Driven by the advice of stakeholders or experts.
- **Regression-averse**: Focused on preventing regression through automation and reuse of test cases.
- **Reactive**: Testing is reactive to system behavior during execution (e.g., exploratory testing).

An appropriate strategy often combines several of these approaches. For example, **risk-based testing** (analytical) can be combined with **exploratory testing** (reactive).

The **test approach** tailors the strategy for a specific project or release, selecting techniques, levels, types, and criteria (entry and exit). It considers project complexity, goals, risks, and resources.

#### 5.2.3 Entry Criteria and Exit Criteria (Definition of Ready and Definition of Done)
**Entry criteria** (or **definition of ready** in Agile) specify the preconditions for starting a test activity. If unmet, testing may become more challenging, costly, or risky. **Exit criteria** (or **definition of done**) define the conditions for declaring a test level or set of tests complete.

Typical **entry criteria** include:
- Availability of **testable requirements**, user stories, or models
- Test items meeting the **exit criteria** for prior levels
