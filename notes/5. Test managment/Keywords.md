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
- **Availability of test environment**
- **Availability of necessary test tools**
- **Availability of test data** and other necessary resources

### Typical Exit Criteria Include:
- Planned tests have been executed
- A defined level of **coverage** (e.g., requirements, user stories, acceptance criteria, risks, code) has been achieved
- The number of unresolved defects is within an agreed limit
- The number of estimated remaining defects is sufficiently low
- The evaluated levels of **reliability**, **performance efficiency**, **usability**, **security**, and other relevant quality characteristics are sufficient

Even if exit criteria are not fully satisfied, testing activities may be curtailed due to constraints such as budget, time, or pressure to release the product. In such cases, it can be acceptable to stop testing if the stakeholders and business owners accept the associated risks of going live without further testing.

### 5.2.4 Test Execution Schedule
Once test cases and procedures are ready, they are assembled into test suites and arranged into a **test execution schedule**, which defines the order in which the suites will run. The execution schedule considers factors such as:
- **Prioritization** of test cases
- **Dependencies** between test cases or features
- **Confirmation** tests
- **Regression** tests

Ideally, test cases are run based on priority, with the highest-priority cases executed first. However, dependencies may require some lower-priority test cases to be executed first. **Confirmation** and **regression tests** also need to be prioritized based on the importance of rapid feedback on changes, but these may also be influenced by dependencies.

Sometimes, different sequences of tests may be possible, and decisions must be made to balance efficiency of execution against strict adherence to prioritization.

### 5.2.5 Factors Influencing the Test Effort
**Test effort estimation** involves predicting the amount of work required to meet testing objectives for a project, release, or iteration. Factors influencing the test effort may include:

#### Product Characteristics:
- The **risks** associated with the product
- The quality of the **test basis**
- The **size** of the product
- **The complexity of the product domain**
- **The requirements for quality characteristics** (e.g., security, reliability)
- The required level of detail for **test documentation**
- Requirements for **legal and regulatory compliance**

#### Development Process Characteristics:
- The stability and maturity of the organization
- The **development model** in use
- The **test approach**
- The tools used
- The **test process**
- **Time pressure**

#### People Characteristics:
- The **skills and experience** of the people involved, especially with similar projects and products (e.g., domain knowledge)
- Team cohesion and **leadership**

#### Test Results:
- The number and severity of **defects** found
- The amount of **rework** required

### 5.2.6 Test Estimation Techniques
Two commonly used techniques for test effort estimation are:

1. **Metrics-based technique**: Estimating the test effort based on metrics from former similar projects or typical values.
  - For example, in Agile development, **burndown charts** are used to track effort remaining and feed into the team's velocity for future iterations.

2. **Expert-based technique**: Estimating the test effort based on the experience of task owners or experts.
  - For example, in Agile development, **planning poker** is used by team members to estimate the effort for delivering features based on experience.

In sequential projects, defect removal models are used as an example of the **metrics-based approach**, while **Wideband Delphi estimation** is an example of the **expert-based approach**.

---

### 5.3 Test Monitoring and Control
The purpose of **test monitoring** is to gather information and provide feedback and visibility about test activities. This information helps assess progress and whether exit criteria are satisfied, such as meeting the targets for coverage of risks, requirements, or acceptance criteria.

**Test control** involves corrective actions based on the metrics gathered. Actions may affect any test activity and other software lifecycle activities.

#### Examples of Test Control Actions:
- **Re-prioritizing tests** due to identified risks (e.g., delayed software delivery)
- **Changing the test schedule** due to resource or environment availability
- **Re-evaluating test items** based on whether they meet entry or exit criteria after rework

### 5.3.1 Metrics Used in Testing
Metrics help assess the progress, quality, and adequacy of test activities. Common test metrics include:

- **Percentage of planned work done** in test case preparation or implementation
- **Percentage of planned work done** in test environment preparation
- **Test case execution** metrics (e.g., number of test cases run/not run, passed/failed)
- **Defect information** (e.g., defect density, defects found and fixed, failure rate, confirmation test results)
- **Test coverage** of requirements, user stories, acceptance criteria, risks, or code
- Task completion, resource allocation, usage, and effort
- **Cost of testing**, including the cost compared to the benefit of finding the next defect or running the next test

### 5.3.2 Purposes, Contents, and Audiences for Test Reports

The purpose of **test reporting** is to summarize and communicate information about test activities, both during and at the end of a test activity (e.g., a test level).

- **Test progress reports**: Prepared during a test activity.
- **Test summary reports**: Prepared at the end of a test activity.

During **test monitoring and control**, the test manager regularly issues test progress reports for stakeholders. These reports provide updates on test progress and any issues encountered.

#### Typical contents of test progress reports:
- Status of test activities and progress against the test plan
- Factors impeding progress
- Planned testing for the next reporting period
- Quality of the test object

When exit criteria are reached, the test manager issues a **test summary report**, summarizing the testing performed based on the latest test progress report and other relevant information.

#### Typical contents of test summary reports:
- Summary of testing performed
- Information on events during the test period
- Deviations from the plan (e.g., schedule, duration, effort)
- Status of testing and product quality with respect to exit criteria or definition of done
- Factors blocking progress
- Metrics of defects, test cases, test coverage, and resource consumption
- **Residual risks** (see section 5.5)
- Reusable test work products produced

The **contents of a test report** will vary based on the project, organizational requirements, and software development lifecycle. For example, a complex project may require more detailed reports than a quick software update. In Agile development, test progress reporting may be done via **task boards**, **defect summaries**, or **burndown charts** and discussed in daily stand-up meetings.

Test reports should also be **tailored to the audience**:
- **Technical audience or test team**: Detailed information, such as defect types and trends, is important.
- **Executive audience**: A high-level report, such as a summary of defects by priority, budget, schedule, and test conditions passed/failed, is more appropriate.

ISO standard (ISO/IEC/IEEE 29119-3) refers to two types of test reports:
1. **Test progress reports**
2. **Test completion reports** (called test summary reports in this syllabus)

The ISO standard also provides structures and examples for each type.
