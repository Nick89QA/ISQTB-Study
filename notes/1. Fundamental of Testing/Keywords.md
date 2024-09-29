# Keywords
- coverage
- debugging
- defect
- error
- failure
- quality
- quality assurance
- root cause
- test analysis
- test basis
- test case
- test completion
- test condition
- test control
- test data
- test design
- test execution
- test implementation
- test monitoring
- test object
- test objective
- test oracle
- test planning
- test procedure
- test process
- test suite
- testing
- testware
- traceability
- validation
- verification

# Learning Objectives for Fundamentals of Testing

## 1.1 What is Testing?

- **FL-1.1.1 (K1)**: Identify typical objectives of testing.
- **FL-1.1.2 (K2)**: Differentiate testing from debugging.

## 1.2 Why is Testing Necessary?

- **FL-1.2.1 (K2)**: Give examples of why testing is necessary.
- **FL-1.2.2 (K2)**: Describe the relationship between testing and quality assurance and give examples of how testing contributes to higher quality.
- **FL-1.2.3 (K2)**: Distinguish between error, defect, and failure.
- **FL-1.2.4 (K2)**: Distinguish between the root cause of a defect and its effects.

## 1.3 Seven Testing Principles

- **FL-1.3.1 (K2)**: Explain the seven testing principles.

## 1.4 Test Process

- **FL-1.4.1 (K2)**: Explain the impact of context on the test process.
- **FL-1.4.2 (K2)**: Describe the test activities and respective tasks within the test process.
- **FL-1.4.3 (K2)**: Differentiate the work products that support the test process.
- **FL-1.4.4 (K2)**: Explain the value of maintaining traceability between the test basis and test work products.

## 1.5 The Psychology of Testing

- **FL-1.5.1 (K1)**: Identify the psychological factors that influence the success of testing.
- **FL-1.5.2 (K2)**: Explain the difference between the mindset required for test activities and the mindset required for development activities.

# 1.1 What is Testing?

Software systems are an integral part of life, from business applications (e.g., banking) to consumer products (e.g., cars). Most people have had an experience with software that did not work as expected. Software that does not work correctly can lead to many problems, including loss of money, time, or business reputation, and even injury or death. Software testing is a way to assess the quality of the software and to reduce the risk of software failure in operation.

A common misperception of testing is that it only consists of running tests, i.e., executing the software and checking the results. As described in section 1.4, software testing is a process that includes many different activities; test execution (including checking of results) is only one of these activities. The test process also includes activities such as test planning, analyzing, designing, and implementing tests, reporting test progress and results, and evaluating the quality of a test object.

Some testing involves the execution of the component or system being tested; such testing is called **dynamic testing**. Other testing does not involve the execution of the component or system being tested; such testing is called **static testing**. Testing also includes reviewing work products such as requirements, user stories, and source code.

Another common misperception of testing is that it focuses entirely on **verification** of requirements, user stories, or other specifications. While testing does involve checking whether the system meets specified requirements, it also involves **validation**, which is checking whether the system will meet user and other stakeholder needs in its operational environment(s).

Test activities are organized and carried out differently in different lifecycles (see section 2.1).

## 1.1.1 Typical Objectives of Testing

For any given project, the objectives of testing may include:

- To prevent defects by evaluating work products such as requirements, user stories, design, and code.
- To verify whether all specified requirements have been fulfilled.
- To check whether the test object is complete and validate if it works as the users and other stakeholders expect.
- To build confidence in the level of quality of the test object.
- To find defects and failures by reducing the level of risk of inadequate software quality.
- To provide sufficient information to stakeholders to allow them to make informed decisions, especially regarding the level of quality of the test object.
- To comply with contractual, legal, or regulatory requirements or standards, and/or to verify the test object’s compliance with such requirements or standards.

The objectives of testing can vary, depending upon the context of the component or system being tested, the test level, and the software development lifecycle model. These differences may include, for example:

- During component testing, one objective may be to find as many failures as possible so that the underlying defects are identified and fixed early. Another objective may be to increase code coverage of the component tests.
- During acceptance testing, one objective may be to confirm that the system works as expected and satisfies requirements. Another objective of this testing may be to give information to stakeholders about the risk of releasing the system at a given time.

## 1.1.2 Testing and Debugging

Testing and debugging are different. Executing tests can show failures that are caused by defects in the software. Debugging is the development activity that finds, analyzes, and fixes such defects. Subsequent confirmation testing checks whether the fixes resolved the defects.

In some cases, testers are responsible for the initial test and the final confirmation test, while developers do the debugging, associated component, and component integration testing. However, in Agile development and in some other software development lifecycles, testers may be involved in debugging and component testing.

## ISO standard (ISO/IEC/IEEE 29119-1) has further information about software testing concepts.

---

## 1.2 Why is Testing Necessary?

Rigorous testing of components and systems, and their associated documentation, can help reduce the risk of failures occurring during operation. When defects are detected, and subsequently fixed, this contributes to the quality of the components or systems. In addition, software testing may also be required to meet contractual or legal requirements or industry-specific standards.

---

### 1.2.1 Testing’s Contributions to Success

Throughout the history of computing, it is quite common for software and systems to be delivered into operation and, due to the presence of defects, to subsequently cause failures or otherwise not meet the stakeholders’ needs. However, using appropriate test techniques can reduce the frequency of such problematic deliveries, when those techniques are applied with the appropriate level of test expertise, in the appropriate test levels, and at the appropriate points in the software development lifecycle. Examples include:

- Having testers involved in requirements reviews or user story refinement could detect defects in these work products. The identification and removal of requirements defects reduces the risk of incorrect or untestable features being developed.
- Having testers work closely with system designers while the system is being designed can increase each party’s understanding of the design and how to test it. This increased understanding can reduce the risk of fundamental design defects and enable tests to be identified at an early stage.
- Having testers work closely with developers while the code is under development can increase each party’s understanding of the code and how to test it. This increased understanding can reduce the risk of defects within the code and the tests.
- Having testers verify and validate the software prior to release can detect failures that might otherwise have been missed, and support the process of removing the defects that caused the failures (i.e., debugging). This increases the likelihood that the software meets stakeholder needs and satisfies requirements.

In addition to these examples, the achievement of defined test objectives (see section 1.1.1) contributes to overall software development and maintenance success.

---

### 1.2.2 Quality Assurance and Testing

While people often use the phrase quality assurance (or just QA) to refer to testing, quality assurance and testing are not the same, but they are related. A larger concept, quality management, ties them together. Quality management includes all activities that direct and control an organization with regard to quality. Among other activities, quality management includes both quality assurance and quality control. Quality assurance is typically focused on adherence to proper processes, in order to provide confidence that the appropriate levels of quality will be achieved. When processes are carried out properly, the work products created by those processes are generally of higher quality, which contributes to defect prevention. In addition, the use of root cause analysis to detect and remove the causes of defects, along with the proper application of the findings of retrospective meetings to improve processes, are important for effective quality assurance.

Quality control involves various activities, including test activities, that support the achievement of appropriate levels of quality. Test activities are part of the overall software development or maintenance process. Since quality assurance is concerned with the proper execution of the entire process, quality assurance supports proper testing. As described in sections 1.1.1 and 1.2.1, testing contributes to the achievement of quality in a variety of ways.

---

### 1.2.3 Errors, Defects, and Failures

A person can make an error (mistake), which can lead to the introduction of a defect (fault or bug) in the software code or in some other related work product. An error that leads to the introduction of a defect in one work product can trigger an error that leads to the introduction of a defect in a related work product. For example, a requirements elicitation error can lead to a requirements defect, which then results in a programming error that leads to a defect in the code.

If a defect in the code is executed, this may cause a failure, but not necessarily in all circumstances. For example, some defects require very specific inputs or preconditions to trigger a failure, which may occur rarely or never.

Errors may occur for many reasons, such as:

- Time pressure
- Human fallibility
- Inexperienced or insufficiently skilled project participants
- Miscommunication between project participants, including miscommunication about requirements and design
- Complexity of the code, design, architecture, the underlying problem to be solved, and/or the technologies used
- Misunderstandings about intra-system and inter-system interfaces, especially when such intra-system and inter-system interactions are large in number
- New, unfamiliar technologies

In addition to failures caused due to defects in the code, failures can also be caused by environmental conditions. For example, radiation, electromagnetic fields, and pollution can cause defects in firmware or influence the execution of software by changing hardware conditions.

## Not all unexpected test results are failures.

False positives may occur due to errors in the way tests were executed, or due to defects in the test data, the test environment, or other testware, or for other reasons. The inverse situation can also occur, where similar errors or defects lead to false negatives. False negatives are tests that do not detect defects that they should have detected; false positives are reported as defects, but aren’t actually defects.

---

### 1.2.4 Defects, Root Causes, and Effects

The root causes of defects are the earliest actions or conditions that contributed to creating the defects. Defects can be analyzed to identify their root causes, so as to reduce the occurrence of similar defects in the future. By focusing on the most significant root causes, root cause analysis can lead to process improvements that prevent a significant number of future defects from being introduced.

For example, suppose incorrect interest payments, due to a single line of incorrect code, result in customer complaints. The defective code was written for a user story which was ambiguous, due to the product owner’s misunderstanding of how to calculate interest. If a large percentage of defects exist in interest calculations, and these defects have their root cause in similar misunderstandings, the product owners could be trained in the topic of interest calculations to reduce such defects in the future.

In this example, the customer complaints are effects. The incorrect interest payments are failures. The improper calculation in the code is a defect, and it resulted from the original defect, the ambiguity in the user story. The root cause of the original defect was a lack of knowledge on the part of the product owner, which resulted in the product owner making an error while writing the user story. The process of root cause analysis is discussed in ISTQB-CTEL-TM and ISTQB-CTEL-ITP.

---

## 1.3 Seven Testing Principles

A number of testing principles have been suggested over the past 50 years and offer general guidelines common for all testing.

### 1. Testing shows the presence of defects, not their absence
Testing can show that defects are present, but cannot prove that there are no defects. Testing reduces the probability of undiscovered defects remaining in the software but, even if no defects are found, testing is not a proof of correctness.

### 2. Exhaustive testing is impossible
Testing everything (all combinations of inputs and preconditions) is not feasible except for trivial cases. Rather than attempting to test exhaustively, risk analysis, test techniques, and priorities should be used to focus test efforts.

### 3. Early testing saves time and money
To find defects early, both static and dynamic test activities should be started as early as possible in the software development lifecycle. Early testing is sometimes referred to as shift left. Testing early in the software development lifecycle helps reduce or eliminate costly changes (see section 3.1).

### 4. Defects cluster together
A small number of modules usually contains most of the defects discovered during pre-release testing, or is responsible for most of the operational failures. Predicted defect clusters, and the actual observed defect clusters in test or operation, are an important input into a risk analysis used to focus the test effort (as mentioned in principle 2).

### 5. Beware of the pesticide paradox
If the same tests are repeated over and over again, eventually these tests no longer find any new defects. To detect new defects, existing tests and test data may need changing, and new tests may need to be written. (Tests are no longer effective at finding defects, just as pesticides are no longer effective at killing insects after a while.) In some cases, such as automated regression testing, the pesticide paradox has a beneficial outcome, which is the relatively low number of regression defects.

### 6. Testing is context dependent
Testing is done differently in different contexts. For example, safety-critical industrial control software is tested differently from an e-commerce mobile app. As another example, testing in an Agile project is done differently than testing in a sequential software development lifecycle project (see section 2.1).

### 7. Absence-of-errors is a fallacy
Some organizations expect that testers can run all possible tests and find all possible defects, but principles 2 and 1, respectively, tell us that this is impossible. Further, it is a fallacy (i.e., a mistaken belief) to expect that just finding and fixing a large number of defects will ensure the success of a system. For example, thoroughly testing all specified requirements and fixing all defects found could still produce a system that is difficult to use, that does not fulfill the users’ needs and expectations, or that is inferior compared to other competing systems.

See Myers 2011, Kaner 2002, Weinberg 2008, and Beizer 1990 for examples of these and other testing principles.

---

## 1.4 Test Process

There is no one universal software test process, but there are common sets of test activities without which testing will be less likely to achieve its established objectives. These sets of test activities are a test process. The proper, specific software test process in any given situation depends on many factors. Which test activities are involved in this test process, how these activities are implemented, and when these activities occur may be discussed in an organization’s test strategy.

---

### 1.4.1 Test Process in Context

Contextual factors that influence the test process for an organization, include, but are not limited to:

- Software development lifecycle model and project methodologies being used
- Test levels and test types being considered
- Product and project risks
- Business domain
- Operational constraints, including but not limited to:
    - Budgets and resources
    - Timescales
    - Complexity
    - Contractual and regulatory requirements
- Organizational policies and practices
- Required internal and external standards

The following sections describe general aspects of organizational test processes in terms of the following:

- Test activities and tasks
- Test work products
- Traceability between the test basis and test work products

It is very useful if the test basis (for any level or type of testing that is being considered) has measurable coverage criteria defined. The coverage criteria can act effectively as key performance indicators (KPIs) to drive the activities that demonstrate achievement of software test objectives (see section 1.1.1).

For example, for a mobile application, the test basis may include a list of requirements and a list of supported mobile devices. Each requirement is an element of the test basis. Each supported device is also an element of the test basis. The coverage criteria may require at least one test case for each element of the test basis. Once executed, the results of these tests tell stakeholders whether specified requirements are fulfilled and whether failures were observed on supported devices.

ISO standard (ISO/IEC/IEEE 29119-2) has further information about test processes.

## 1.4.2 Test Activities and Tasks

A test process consists of the following main groups of activities:
- Test planning
- Test monitoring and control
- Test analysis
- Test design
- Test implementation
- Test execution
- Test completion

Each main group of activities is composed of constituent activities, which will be described in the subsections below. Each constituent activity consists of multiple individual tasks, which would vary from one project or release to another.

Further, although many of these main activity groups may appear logically sequential, they are often implemented iteratively. For example, Agile development involves small iterations of software design, build, and test that happen on a continuous basis, supported by ongoing planning. So test activities are also happening on an iterative, continuous basis within this software development approach. Even in sequential software development, the stepped logical sequence of main groups of activities will involve overlap, combination, concurrency, or omission, so tailoring these main groups of activities within the context of the system and the project is usually required.

---

### Test Planning

Test planning involves activities that define the objectives of testing and the approach for meeting test objectives within constraints imposed by the context (e.g., specifying suitable test techniques and tasks, and formulating a test schedule for meeting a deadline). Test plans may be revisited based on feedback from monitoring and control activities. Test planning is further explained in section 5.2.

---

### Test Monitoring and Control

Test monitoring involves the ongoing comparison of actual progress against planned progress using any test monitoring metrics defined in the test plan. Test control involves taking actions necessary to meet the objectives of the test plan (which may be updated over time). Test monitoring and control are supported by the evaluation of exit criteria, which are referred to as the definition of done in some software development lifecycle models (see ISTQB-CTFL-AT). For example, the evaluation of exit criteria for test execution as part of a given test level may include:

- Checking test results and logs against specified coverage criteria
- Assessing the level of component or system quality based on test results and logs
- Determining if more tests are needed (e.g., if tests originally intended to achieve a certain level of product risk coverage failed to do so, requiring additional tests to be written and executed)

Test progress against the plan is communicated to stakeholders in test progress reports, including deviations from the plan and information to support any decision to stop testing.

Test monitoring and control are further explained in section 5.3.

---

### Test Analysis

During test analysis, the test basis is analyzed to identify testable features and define associated test conditions. In other words, test analysis determines “what to test” in terms of measurable coverage criteria.

Test analysis includes the following major activities:

- Analyzing the test basis appropriate to the test level being considered, for example:
  - Requirement specifications, such as business requirements, functional requirements, system requirements, user stories, epics, use cases, or similar work products that specify desired functional and non-functional component or system behavior
  - Design and implementation information, such as system or software architecture diagrams or documents, design specifications, call flow graphs, modeling diagrams (e.g., UML or entity-relationship diagrams), interface specifications, or similar work products that specify component or system structure
  - The implementation of the component or system itself, including code, database metadata and queries, and interfaces
  - Risk analysis reports, which may consider functional, non-functional, and structural aspects of the component or system

- Evaluating the test basis and test items to identify defects of various types, such as:
  - Ambiguities
  - Omissions
  - Inconsistencies
  - Inaccuracies
  - Contradictions
  - Superfluous statements
  
- Identifying features and sets of features to be tested
- Defining and prioritizing test conditions for each feature based on analysis of the test basis, and considering functional, non-functional, and structural characteristics, other business and technical factors, and levels of risks
- Capturing bi-directional traceability between each element of the test basis and the associated test conditions (see sections 1.4.3 and 1.4.4)

The application of black-box, white-box, and experience-based test techniques can be useful in the process of test analysis (see chapter 4) to reduce the likelihood of omitting important test conditions and to define more precise and accurate test conditions.

In some cases, test analysis produces test conditions which are to be used as test objectives in test charters. Test charters are typical work products in some types of experience-based testing (see section 4.4.2). When these test objectives are traceable to the test basis, coverage achieved during such experience-based testing can be measured.

The identification of defects during test analysis is an important potential benefit, especially where no other review process is being used and/or the test process is closely connected with the review process. Such test analysis activities not only verify whether the requirements are consistent, properly expressed, and complete, but also validate whether the requirements properly capture customer, user, and other stakeholder needs. For example, techniques such as behavior driven development (BDD) and acceptance test driven development (ATDD), which involve generating test conditions and test cases from user stories and acceptance criteria prior to coding. These techniques also verify, validate, and detect defects in the user stories and acceptance criteria (see ISTQB-CTFL-AT).

---

### Test Design

During test design, the test conditions are elaborated into high-level test cases, sets of high-level test cases, and other testware. So, test analysis answers the question “what to test?” while test design answers the question “how to test?”

Test design includes the following major activities:
- Designing and prioritizing test cases and sets of test cases
- Identifying necessary test data to support test conditions and test cases
- Designing the test environment and identifying any required infrastructure and tools
- Capturing bi-directional traceability between the test basis, test conditions, and test cases (see section 1.4.4)

The elaboration of test conditions into test cases and sets of test cases during test design often involves using test techniques (see chapter 4).

As with test analysis, test design may also result in the identification of similar types of defects in the test basis. Also, as with test analysis, the identification of defects during test design is an important potential benefit.

### Test Implementation

During test implementation, the testware necessary for test execution is created and/or completed, including sequencing the test cases into test procedures. So, test design answers the question “how to test?” while test implementation answers the question “do we now have everything in place to run the tests?”

Test implementation includes the following major activities:

- Developing and prioritizing test procedures, and, potentially, creating automated test scripts
- Creating test suites from the test procedures and (if any) automated test scripts
- Arranging the test suites within a test execution schedule in a way that results in efficient test execution (see section 5.2.4)
- Building the test environment (including, potentially, test harnesses, service virtualization, simulators, and other infrastructure items) and verifying that everything needed has been set up correctly
- Preparing test data and ensuring it is properly loaded in the test environment
- Verifying and updating bi-directional traceability between the test basis, test conditions, test cases, test procedures, and test suites (see section 1.4.4)

Test design and test implementation tasks are often combined.

In exploratory testing and other types of experience-based testing, test design and implementation may occur, and may be documented, as part of test execution. Exploratory testing may be based on test charters (produced as part of test analysis), and exploratory tests are executed immediately as they are designed and implemented (see section 4.4.2).

---

### Test Execution

During test execution, test suites are run in accordance with the test execution schedule. Test execution includes the following major activities:

- Recording the IDs and versions of the test item(s) or test object, test tool(s), and testware
- Executing tests either manually or by using test execution tools
- Comparing actual results with expected results
- Analyzing anomalies to establish their likely causes (e.g., failures may occur due to defects in the code, but false positives also may occur, see section 1.2.3)
- Reporting defects based on the failures observed (see section 5.6)
- Logging the outcome of test execution (e.g., pass, fail, blocked)
- Repeating test activities either as a result of action taken for an anomaly, or as part of the planned testing (e.g., execution of a corrected test, confirmation testing, and/or regression testing)
- Verifying and updating bi-directional traceability between the test basis, test conditions, test cases, test procedures, and test results

---

### Test Completion

Test completion activities collect data from completed test activities to consolidate experience, testware, and any other relevant information. Test completion activities occur at project milestones such as when a software system is released, a test project is completed (or cancelled), an Agile project iteration is finished, a test level is completed, or a maintenance release has been completed.

Test completion includes the following major activities:

- Checking whether all defect reports are closed, entering change requests or product backlog items for any defects that remain unresolved at the end of test execution
- Creating a test summary report to be communicated to stakeholders
- Finalizing and archiving the test environment, the test data, the test infrastructure, and other testware for later reuse
- Handing over the testware to the maintenance teams, other project teams, and/or other stakeholders who could benefit from its use
- Analyzing lessons learned from the completed test activities to determine changes needed for future iterations, releases, and projects
- Using the information gathered to improve test process maturity

---
### Test Work Products

Test work products are created as part of the test process. Just as there is significant variation in the way that organizations implement the test process, there is also significant variation in the types of work products created during that process, in the ways those work products are organized and managed, and in the names used for those work products. This syllabus adheres to the test process outlined above, and the work products described in this syllabus and in the ISTQB® Glossary. The ISO standard (ISO/IEC/IEEE 29119-3) may also serve as a guideline for test work products.

Many of the test work products described in this section can be captured and managed using test management tools and defect management tools (see chapter 6).

#### Test Planning Work Products

Test planning work products typically include one or more test plans. The test plan includes information about the test basis, to which the other test work products will be related via traceability information (see below and section 1.4.4), as well as exit criteria (or definition of done) which will be used during test monitoring and control. Test plans are described in section 5.2.

#### Test Monitoring and Control Work Products

Test monitoring and control work products typically include various types of test reports, including test progress reports produced on an ongoing and/or a regular basis, and test summary reports produced at various completion milestones. All test reports should provide audience-relevant details about the test progress as of the date of the report, including summarizing the test execution results once those become available.

Test monitoring and control work products should also address project management concerns, such as task completion, resource allocation and usage, and effort.

Test monitoring and control, and the work products created during these activities, are further explained in section 5.3 of this syllabus.

### Test Analysis Work Products

Test analysis work products include defined and prioritized test conditions, each of which is ideally bi-directionally traceable to the specific element(s) of the test basis it covers. For exploratory testing, test analysis may involve the creation of test charters. Test analysis may also result in the discovery and reporting of defects in the test basis.

---

### Test Design Work Products

Test design results in test cases and sets of test cases to exercise the test conditions defined in test analysis. It is often a good practice to design high-level test cases, without concrete values for input data and expected results. Such high-level test cases are reusable across multiple test cycles with different concrete data, while still adequately documenting the scope of the test case. Ideally, each test case is bi-directionally traceable to the test condition(s) it covers.

Test design also results in:

- The design and/or identification of the necessary test data
- The design of the test environment
- The identification of infrastructure and tools

Though the extent to which these results are documented varies significantly.

---

### Test Implementation Work Products

Test implementation work products include:

- Test procedures and the sequencing of those test procedures
- Test suites
- A test execution schedule

Ideally, once test implementation is complete, achievement of coverage criteria established in the test plan can be demonstrated via bi-directional traceability between test procedures and specific elements of the test basis, through the test cases and test conditions.

In some cases, test implementation involves creating work products using or used by tools, such as service virtualization and automated test scripts.

Test implementation may also result in the creation and verification of test data and the test environment. The completeness of the documentation of the data and/or environment verification results may vary significantly.

The test data serve to assign concrete values to the inputs and expected results of test cases. Such concrete values, together with explicit directions about the use of the concrete values, turn high-level test cases into executable low-level test cases. The same high-level test case may use different test data when executed on different releases of the test object. The concrete expected results which are associated with concrete test data are identified by using a test oracle.

In exploratory testing, some test design and implementation work products may be created during test execution, though the extent to which exploratory tests (and their traceability to specific elements of the test basis) are documented may vary significantly.

Test conditions defined in test analysis may be further refined in test implementation.

### Test Execution Work Products

Test execution work products include:

- Documentation of the status of individual test cases or test procedures (e.g., ready to run, pass, fail, blocked, deliberately skipped, etc.)
- Defect reports (see section 5.6)
- Documentation about which test item(s), test object(s), test tools, and testware were involved in the testing

Ideally, once test execution is complete, the status of each element of the test basis can be determined and reported via bi-directional traceability with the associated test procedure(s). For example, we can say which requirements have passed all planned tests, which requirements have failed tests and/or have defects associated with them, and which requirements have planned tests still waiting to be run. This enables verification that the coverage criteria have been met, and allows for reporting test results in terms that are understandable to stakeholders.

---

### Test Completion Work Products

Test completion work products include:

- Test summary reports
- Action items for improvement of subsequent projects or iterations
- Change requests or product backlog items
- Finalized testware

---

### Traceability Between the Test Basis and Test Work Products

As mentioned in section 1.4.3, test work products and the names of those work products vary significantly. Regardless of these variations, in order to implement effective test monitoring and control, it is important to establish and maintain traceability throughout the test process between each element of the test basis and the various test work products associated with that element.

In addition to the evaluation of test coverage, good traceability supports:

- Analyzing the impact of changes
- Making testing auditable
- Meeting IT governance criteria
- Improving the understandability of test progress reports and test summary reports to include the status of elements of the test basis (e.g., requirements that passed their tests, requirements that failed their tests, and requirements that have pending tests)
- Relating the technical aspects of testing to stakeholders in terms that they can understand
- Providing information to assess product quality, process capability, and project progress against business goals

Some test management tools provide test work product models that match part or all of the test work products outlined in this section. Some organizations build their own management systems to organize the work products and provide the information traceability they require.
### 1.5 The Psychology of Testing

Software development, including software testing, involves human beings. Therefore, human psychology has important effects on software testing.

---

#### 1.5.1 Human Psychology and Testing

Identifying defects during a static test (e.g., a requirement review or user story refinement session), or identifying failures during dynamic test execution, may be perceived as criticism of the product and its author. **Confirmation bias**, a cognitive bias, can make it difficult to accept information that disagrees with one's currently held beliefs. For instance, developers expect their code to be correct, leading to a bias that makes it hard to accept that their code is faulty. Other cognitive biases can similarly affect how people perceive information from testing.

Moreover, people often tend to "blame the bearer of bad news," and since testing can often reveal negative information, it may be viewed as a destructive activity, despite its critical role in ensuring project success and product quality (see sections 1.1 and 1.2).

To minimize these negative perceptions, communication about defects and failures should be done constructively, helping reduce tensions between testers, analysts, product owners, designers, and developers. This applies to both static and dynamic testing.

Testers and test managers need to develop good interpersonal skills to communicate effectively about defects, failures, test results, test progress, and risks, and to foster positive relationships with colleagues.

Examples of good communication include:

- **Start with collaboration**: Remind everyone of the shared goal of delivering better quality systems.
- **Emphasize the benefits of testing**: For authors, defect information helps them improve their work and skills. For the organization, defects caught during testing save time, money, and reduce risks to product quality.
- **Communicate test results neutrally**: Present findings in a fact-focused, non-critical manner. Write objective, factual defect reports and review findings.
- **Understand reactions**: Be empathetic towards any negative reactions to the information.
- **Ensure mutual understanding**: Confirm both sides have understood the conversation.

Setting the right test objectives, as discussed earlier (see section 1.1), also has psychological implications. People tend to align their behavior with the team's and stakeholders' objectives. It's important that testers follow these objectives without personal bias.

---

#### 1.5.2 Tester’s and Developer’s Mindsets

Developers and testers often have different mindsets. The primary objective of development is to design and build a product, whereas the objectives of testing involve verifying and validating the product, finding defects before release, and more. These differing objectives require different mindsets. Aligning these mindsets can lead to higher product quality.

A mindset is shaped by an individual’s assumptions and preferred methods for decision-making and problem-solving. A **tester’s mindset** should include:

- Curiosity
- Professional pessimism
- A critical eye
- Attention to detail
- Motivation for positive communication and relationships

A tester’s mindset grows and matures with experience.

On the other hand, **a developer’s mindset** might share some traits with a tester's but focuses more on designing and building solutions, rather than considering potential flaws. **Confirmation bias** also makes it hard for developers to see their own errors.

With the right mindset, developers can test their own code. Different software development lifecycle models organize testers and test activities differently. Independent testers can increase defect detection effectiveness, especially for large, complex, or safety-critical systems. **Independent testers** offer a perspective different from the authors (e.g., business analysts, product owners, designers, developers) because they have different cognitive biases.
