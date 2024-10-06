### Keywords

- **Acceptance Testing**
- **Alpha Testing**
- **Beta Testing**
- **Change-related Testing**
- **Commercial Off-the-shelf (COTS)**
- **Component Integration Testing**
- **Component Testing**
- **Confirmation Testing**
- **Contractual Acceptance Testing**
- **Functional Testing**
- **Impact Analysis**
- **Integration Testing**
- **Maintenance Testing**
- **Non-functional Testing**
- **Operational Acceptance Testing**
- **Regression Testing**
- **Regulatory Acceptance Testing**
- **Sequential Development Model**
- **System Integration Testing**
- **System Testing**
- **Test Basis**
- **Test Case**
- **Test Environment**
- **Test Level**
- **Test Object**
- **Test Objective**
- **Test Type**
- **User Acceptance Testing**
- **White-box Testing**

---

### Learning Objectives for Testing Throughout the Software Development Lifecycle

#### 2.1 Software Development Lifecycle Models

- **FL-2.1.1 (K2)**: Explain the relationships between software development activities and test activities in the software development lifecycle.
- **FL-2.1.2 (K1)**: Identify reasons why software development lifecycle models must be adapted to the context of project and product characteristics.

#### 2.2 Test Levels

- **FL-2.2.1 (K2)**: Compare the different test levels from the perspective of objectives, test basis, test objects, typical defects and failures, and approaches and responsibilities.

#### 2.3 Test Types

- **FL-2.3.1 (K2)**: Compare functional, non-functional, and white-box testing.
- **FL-2.3.2 (K1)**: Recognize that functional, non-functional, and white-box tests occur at any test level.
- **FL-2.3.3 (K2)**: Compare the purposes of confirmation testing and regression testing.

#### 2.4 Maintenance Testing

- **FL-2.4.1 (K2)**: Summarize triggers for maintenance testing.
- **FL-2.4.2 (K2)**: Describe the role of impact analysis in maintenance testing.

---

### 2.1 Software Development Lifecycle Models

A software development lifecycle model outlines the activities at each stage of a software project and how these activities relate to one another. Different models require different approaches to testing.

#### 2.1.1 Software Development and Software Testing

A tester's role includes familiarity with the common software development lifecycle models to ensure appropriate test activities. Important characteristics of good testing in any lifecycle model include:

- Corresponding test activity for each development activity.
- Each test level has objectives specific to that level.
- Test analysis and design start during the corresponding development activity.
- Testers participate in defining and refining requirements, design, and reviewing work products (e.g., requirements, design, user stories) as early as possible.

Test activities should begin early in the lifecycle, adhering to the principle of early testing.

#### Sequential Development Models

Sequential development models describe a linear flow of activities where one phase begins when the previous one ends. Examples include:

- **Waterfall Model**: Development activities such as requirements analysis, design, coding, and testing are completed sequentially, with testing occurring only after all development activities.
- **V-Model**: Integrates the test process throughout development and includes test levels corresponding to each development phase. Test execution may overlap in some cases.

Sequential models deliver software with a complete set of features but often require months or years for delivery.

#### Iterative and Incremental Development Models

In **incremental development**, the system grows piece by piece, with each feature increment varying in size.

In **iterative development**, features are specified, designed, built, and tested in cycles of fixed duration. Iterations may involve revising previously developed features. Examples include:

- **Rational Unified Process**: Long iterations (2-3 months), large feature increments.
- **Scrum**: Short iterations (hours to weeks), small feature increments.
- **Kanban**: Can be implemented with or without fixed-length iterations.
- **Spiral**: Involves experimental increments, which may be reworked or abandoned.

In these models, test levels overlap and iterate. Continuous delivery or deployment often involves significant automation of multiple test levels. Testing evolves as the system grows, with regression testing becoming crucial.

Unlike sequential models, these models deliver usable software quickly but may take months or years to complete all requirements.

#### 2.1.2 Software Development Lifecycle Models in Context

The choice of a lifecycle model depends on the project and product characteristics, business priorities, and risks. For instance, developing a minor internal system is different from developing a safety-critical system.

Teams may need to adapt test levels and activities based on project needs. For example, integrating a COTS product into a larger system may require interoperability testing at the system integration level.

(e.g., integration to the infrastructure and other systems) and at the acceptance test level (functional and non-functional, along with user acceptance testing and operational acceptance testing). See section 2.2 for a discussion of test levels and section 2.3 for a discussion of test types.

In addition, software development lifecycle models themselves may be combined. For example, a V-model may be used for the development and testing of the backend systems and their integrations, while an Agile development model may be used to develop and test the front-end user interface (UI) and functionality. Prototyping may be used early in a project, with an incremental development model adopted once the experimental phase is complete.

**Internet of Things (IoT) systems**, which consist of many different objects, such as devices, products, and services, typically apply separate software development lifecycle models for each object. This presents a particular challenge for the development of Internet of Things system versions. Additionally, the software development lifecycle of such objects places stronger emphasis on the later phases of the software development lifecycle after they have been introduced to operational use (e.g., operate, update, and decommission phases).

Reasons why software development models must be adapted to the context of project and product characteristics include:
- Differences in product risks of systems (complex or simple project)
- Many business units involved in a project or program (combination of sequential and agile development)
- Short time to deliver a product to the market (merging of test levels and/or integration of test types into test levels)

### 2.2 Test Levels

**Test levels** are groups of test activities that are organized and managed together. Each test level is an instance of the test process, consisting of the activities described in section 1.4, performed in relation to software at a given level of development, from individual units or components to complete systems or, where applicable, systems of systems. Test levels are related to other activities within the software development lifecycle.

The test levels used in this syllabus are:
- Component testing
- Integration testing
- System testing
- Acceptance testing

Test levels are characterized by the following attributes:
- Specific objectives
- Test basis, referenced to derive test cases
- Test object (i.e., what is being tested)
- Typical defects and failures
- Specific approaches and responsibilities

For every test level, a suitable test environment is required. For example, in **acceptance testing**, a production-like test environment is ideal, while in **component testing**, the developers typically use their own development environment.

#### 2.2.1 Component Testing

**Objectives of component testing:**

Component testing (also known as unit or module testing) focuses on components that are separately testable. Objectives of component testing include:
- Reducing risk
- Verifying whether the functional and non-functional behaviors of the component are as designed and specified
- Building confidence in the component’s quality
- Finding defects in the component
- Preventing defects from escaping to higher test levels

In some cases, especially in incremental and iterative development models (e.g., Agile), where code changes are ongoing, automated component regression tests play a key role in building confidence that changes have not broken existing components.

Component testing is often done in isolation from the rest of the system, depending on the software development lifecycle model and the system, which may require mock objects, service virtualization, harnesses, stubs, and drivers. Component testing may cover functionality (e.g., correctness of calculations), non-functional characteristics (e.g., searching for memory leaks), and structural properties (e.g., decision testing).

**Test basis:**

Examples of work products that can be used as a test basis for component testing include:
- Detailed design
- Code
- Data model
- Component specifications

**Test objects:**

Typical test objects for component testing include:
- Components, units, or modules
- Code and data structures
- Classes
- Database modules

**Typical defects and failures:**

Examples of typical defects and failures for component testing include:
- Incorrect functionality (e.g., not as described in design specifications)
- Data flow problems
- Incorrect code and logic

Defects are typically fixed as soon as they are found, often with no formal defect management. However, when developers do report defects, this provides important information for root cause analysis and process improvement.

**Specific approaches and responsibilities:**

Component testing is usually performed by the developer who wrote the code, but it at least requires access to the code being tested. Developers may alternate between component development and defect fixing. Developers will often write and execute tests after having written the code for a component. However, in Agile development especially, writing automated component test cases may precede writing application code.

For example, consider test-driven development (TDD). **Test-driven development** is highly iterative and based on cycles of developing automated test cases, then building and integrating small pieces of code, then executing the component tests, correcting any issues, and refactoring the code. This process continues until the component has been completely built and all component tests are passing. Test-driven development is an example of a test-first approach. While TDD originated in eXtreme Programming (XP), it has spread to other forms of Agile and also to sequential lifecycles (see ISTQB-CTFL-AT).

### 2.2.2 Integration Testing

**Objectives of integration testing:**

Integration testing focuses on interactions between components or systems. Objectives of integration testing include:
- Reducing risk
- Verifying whether the functional and non-functional behaviors of the interfaces are as designed and specified
- Building confidence in the quality of the interfaces
- Finding defects (which may be in the interfaces themselves or within the components or systems)
- Preventing defects from escaping to higher test levels

As with component testing, in some cases automated integration regression tests provide confidence that changes have not broken existing interfaces, components, or systems.

There are two different levels of integration testing described in this syllabus, which may be carried out on test objects of varying size as follows:
- **Component integration testing** focuses on the interactions and interfaces between integrated components. Component integration testing is performed after component testing, and is generally automated. In iterative and incremental development, component integration tests are usually part of the continuous integration process.
- **System integration testing** focuses on the interactions and interfaces between systems, packages, and microservices. System integration testing can also cover interactions with, and interfaces provided by, external organizations (e.g., web services). In this case, the developing organization does not control the external interfaces, which can create various challenges for testing (e.g., ensuring that test-blocking defects in the external organization’s code are resolved, arranging for test environments, etc.). System integration testing may be done after system testing or in parallel with ongoing system test activities (in both sequential development and iterative and incremental development).

**Test basis:**

Examples of work products that can be used as a test basis for integration testing include:
- Software and system design
- Sequence diagrams
- Interface and communication protocol specifications
- Use cases
- Architecture at component or system level
- Workflows
- External interface definitions

**Test objects:**

Typical test objects for integration testing include:
- Subsystems
- Databases
- Infrastructure
- Interfaces
- APIs
- Microservices

**Typical defects and failures:**

Examples of typical defects and failures for component integration testing include:
- Incorrect data, missing data, or incorrect data encoding
- Incorrect sequencing or timing of interface calls
- Interface mismatch
- Failures in communication between components
- Unhandled or improperly handled communication failures between components
- Incorrect assumptions about the meaning, units, or boundaries of the data being passed between components

Examples of typical defects and failures for system integration testing include:
- Inconsistent message structures between systems
- Incorrect data, missing data, or incorrect data encoding
- Interface mismatch
- Failures in communication between systems
- Unhandled or improperly handled communication failures between systems

• Incorrect assumptions about the meaning, units, or boundaries of the data being passed between systems
• Failure to comply with mandatory security regulations

**Specific approaches and responsibilities:**

Component integration tests and system integration tests should concentrate on the integration itself. For example, if integrating module A with module B, tests should focus on the communication between the modules, not the functionality of the individual modules, as that should have been covered during component testing. If integrating system X with system Y, tests should focus on the communication between the systems, not the functionality of the individual systems, as that should have been covered during system testing. Both functional, non-functional, and structural test types are applicable.

Component integration testing is often the responsibility of developers, whereas system integration testing is generally the responsibility of testers. Ideally, testers performing system integration testing should understand the system architecture and should have influenced integration planning.

If integration tests and the integration strategy are planned before components or systems are built, those components or systems can be built in the order required for the most efficient testing. Systematic integration strategies may be based on the system architecture (e.g., top-down or bottom-up), functional tasks, transaction processing sequences, or other aspects of the system or components. To simplify defect isolation and detect defects early, integration should typically be incremental (i.e., a small number of components or systems at a time) rather than using the “big bang” approach (i.e., integrating all components or systems in one single step). A risk analysis of the most complex interfaces can help focus the integration testing.

The larger the scope of integration, the more difficult it becomes to isolate defects to a specific component or system, leading to increased risk and additional time for troubleshooting. This is one reason continuous integration, where software is integrated on a component-by-component basis (i.e., functional integration), has become a common practice. Continuous integration often includes automated regression testing, ideally at multiple test levels.

### 2.2.3 System Testing

**Objectives of system testing:**

System testing focuses on the behavior and capabilities of a complete system or product, often considering the end-to-end tasks the system can perform and the non-functional behaviors it exhibits while performing those tasks. Objectives of system testing include:
- Reducing risk
- Verifying whether the functional and non-functional behaviors of the system are as designed and specified
- Validating that the system is complete and will work as expected
- Building confidence in the quality of the system as a whole
- Finding defects
- Preventing defects from escaping to higher test levels or production

For certain systems, verifying data quality may also be an objective. As with component testing and integration testing, automated system regression tests provide confidence that changes have not broken existing features or end-to-end capabilities. System testing often produces information that stakeholders use to make release decisions. System testing may also satisfy legal or regulatory requirements or standards.

The test environment should ideally correspond to the final target or production environment.

**Test basis:**

Examples of work products that can be used as a test basis for system testing include:
- System and software requirement specifications (functional and non-functional)
- Risk analysis reports
- Use cases
- Epics and user stories
- Models of system behavior
- State diagrams
- System and user manuals

**Test objects:**

Typical test objects for system testing include:
- Applications
- Hardware/software systems
- Operating systems
- System under test (SUT)
- System configuration and configuration data

**Typical defects and failures:**

Examples of typical defects and failures for system testing include:
- Incorrect calculations
- Incorrect or unexpected system functional or non-functional behavior
- Incorrect control and/or data flows within the system
- Failure to properly and completely carry out end-to-end functional tasks
- Failure of the system to work properly in the system environment(s)
- Failure of the system to work as described in system and user manuals

**Specific approaches and responsibilities:**

System testing should focus on the overall, end-to-end behavior of the system as a whole, both functional and non-functional. System testing should use the most appropriate techniques for the aspect(s) of the system to be tested. For example, a decision table may be created to verify whether functional behavior is as described in business rules.

System testing is typically carried out by independent testers who rely heavily on specifications. Defects in specifications (e.g., missing user stories, incorrectly stated business requirements, etc.) can lead to misunderstandings or disagreements about expected system behavior. Such situations can cause false positives and false negatives, which waste time and reduce defect detection effectiveness. Early involvement of testers in user story refinement or static testing activities, such as reviews, helps reduce the incidence of such situations.

### 2.2.4 Acceptance Testing

**Objectives of acceptance testing:**

Acceptance testing, like system testing, typically focuses on the behavior and capabilities of a whole system or product. Objectives of acceptance testing include:
- Establishing confidence in the quality of the system as a whole
- Validating that the system is complete and will work as expected
- Verifying that functional and non-functional behaviors of the system are as specified

Acceptance testing may produce information to assess the system’s readiness for deployment and use by the customer (end-user). Defects may be found during acceptance testing, but finding defects is often not an objective, and finding a significant number of defects during acceptance testing may be considered a major project risk. Acceptance testing may also satisfy legal or regulatory requirements or standards.

Common forms of acceptance testing include the following:
- **User acceptance testing**
- **Operational acceptance testing**
- **Contractual and regulatory acceptance testing**
- **Alpha and beta testing**

Each of these forms is described in the following subsections:

#### User Acceptance Testing (UAT)

User acceptance testing typically focuses on validating the fitness for use of the system by intended users in a real or simulated operational environment. The main objective is building confidence that users can use the system to meet their needs, fulfill requirements, and perform business processes with minimal difficulty, cost, and risk.

#### Operational Acceptance Testing (OAT)

Operational acceptance testing is usually performed by operations or systems administration staff in a (simulated) production environment. The tests focus on operational aspects and may include:
- Testing of backup and restore
- Installing, uninstalling, and upgrading
- Disaster recovery
- User management
- Maintenance tasks


**Regulatory acceptance testing** ensures compliance with regulations such as governmental, legal, or safety standards. It is often performed by users or independent testers, sometimes with the results witnessed or audited by regulatory agencies.

The main objective of contractual and regulatory acceptance testing is to ensure that contractual or regulatory compliance has been achieved.

### Alpha and Beta Testing

**Alpha and beta testing** are typically conducted by developers of commercial off-the-shelf (COTS) software to gather feedback from potential or existing users, customers, and/or operators before the product is released to the market.

- **Alpha testing** is performed at the developer's site, typically by potential or existing customers, operators, or an independent test team (but not by the development team itself).
- **Beta testing** is conducted by potential or existing customers and operators in their own environments. Beta testing can occur after alpha testing or independently.

The objectives of alpha and beta testing are to build confidence among potential customers and operators that they can use the system under normal conditions and in operational environments with minimal difficulty, cost, and risk. Another objective is to detect defects related to the conditions and environments in which the system will be used, especially if those conditions are difficult for the development team to replicate.

### Test Basis

Examples of work products that can serve as a test basis for any form of acceptance testing include:
- Business processes
- User or business requirements
- Regulations, legal contracts, and standards
- Use cases and/or user stories
- System requirements
- System or user documentation
- Installation procedures
- Risk analysis reports

For **operational acceptance testing**, specific work products used as a test basis may include:
- Backup and restore procedures
- Disaster recovery procedures
- Non-functional requirements
- Operations documentation
- Deployment and installation instructions
- Performance targets
- Database packages
- Security standards or regulations

### Typical Test Objects

Common test objects for any form of acceptance testing include:
- The system under test (SUT)
- System configuration and configuration data
- Business processes for a fully integrated system
- Recovery systems and hot sites (for business continuity and disaster recovery testing)
- Operational and maintenance processes
- Forms and reports
- Existing and converted production data

### Typical Defects and Failures

Examples of typical defects for any form of acceptance testing include:
- System workflows that do not meet business or user requirements
- Business rules not implemented correctly
- System failing to meet contractual or regulatory requirements
- Non-functional failures, such as security vulnerabilities, inadequate performance efficiency under high loads, or improper operation on a supported platform

### Specific Approaches and Responsibilities

Acceptance testing is typically the responsibility of the customers, business users, product owners, or system operators, though other stakeholders may be involved as well.

Acceptance testing is often considered the final test level in a sequential development lifecycle but may also occur at other times, such as:
- Acceptance testing of a COTS product may happen during installation or integration.
- Acceptance testing of a new functional enhancement may occur before system testing.

In iterative development, project teams may perform various forms of acceptance testing during and at the end of each iteration, such as verifying new features against acceptance criteria or validating that the features meet users’ needs. Alpha and beta tests may also occur at the end of an iteration, after completing an iteration, or after several iterations. User acceptance tests, operational acceptance tests, regulatory acceptance tests, and contractual acceptance tests may also occur at the end of iterations or after multiple iterations.

## 2.3 Test Types

A test type is a group of test activities designed to evaluate specific characteristics of a software system or its components based on particular test objectives. Test objectives may include:
- Evaluating **functional quality characteristics**, such as completeness, correctness, and appropriateness
- Evaluating **non-functional quality characteristics**, such as reliability, performance efficiency, security, compatibility, and usability
- Evaluating the structure or architecture of the system or component to ensure correctness, completeness, and adherence to specifications
- Evaluating the effects of changes, such as confirming defect fixes (confirmation testing) and checking for unintended changes caused by software or environmental changes (regression testing)

### 2.3.1 Functional Testing

**Functional testing** involves testing the functions that a system should perform. Functional requirements may be specified in documents such as business requirements, epics, user stories, use cases, or functional specifications, or they may be undocumented. Functional testing evaluates "what" the system should do.

Functional tests should be performed at all test levels. For example, tests for components may be based on component specifications, though the focus varies across levels.

Since functional testing focuses on the software's behavior, **black-box techniques** can be used to derive test conditions and test cases for the system’s functionality (see section 4.2).

**Functional coverage** measures the thoroughness of functional testing. It indicates the extent to which system functionality has been exercised by tests and is expressed as a percentage of the elements covered. For example, traceability between tests and functional requirements can help calculate the percentage of requirements covered by tests, potentially identifying coverage gaps.

### Functional Test Design and Execution
Functional test design and execution may require specialized skills or knowledge, such as an understanding of the specific business problem the software addresses (e.g., geological modeling software for the oil and gas industries).

### 2.3.2 Non-functional Testing
Non-functional testing evaluates system characteristics such as usability, performance efficiency, or security. According to the ISO standard (ISO/IEC 25010), non-functional testing assesses "how well" a system behaves.

Contrary to common perceptions, non-functional testing should be done at all test levels and as early as possible. Discovering non-functional defects late in the project can severely affect its success.

Black-box techniques (see section 4.2) can be applied to derive test conditions and cases for non-functional testing. For example, boundary value analysis can define stress conditions for performance tests.

The thoroughness of non-functional testing can be measured by **non-functional coverage**, expressed as a percentage of the elements covered by tests. For instance, traceability between tests and supported devices for a mobile application can calculate the percentage of devices covered by compatibility testing, helping to identify coverage gaps.

Non-functional test design and execution may involve special expertise, such as knowledge of potential design weaknesses (e.g., security vulnerabilities in specific programming languages) or user base personas (e.g., users of healthcare facility management systems).

For more information on testing non-functional quality characteristics, refer to ISTQB-CTAL-TA, ISTQB-CTAL-TTA, ISTQB-CTAL-SEC, and other ISTQB® specialist modules.

### 2.3.3 White-box Testing
White-box testing is based on the system's internal structure or implementation, including code, architecture, workflows, and/or data flows (see section 4.3).

**Structural coverage** measures white-box testing thoroughness. It indicates the extent to which structural elements have been exercised by tests, expressed as a percentage. At the component level, code coverage might be measured by the percentage of executable statements tested. At the component integration level, coverage might be measured by the percentage of interfaces exercised by tests.

White-box test design and execution may require expertise in coding, data storage (e.g., database queries), and understanding coverage tools.

### 2.3.4 Change-related Testing
When a system undergoes changes, either to fix defects or introduce new functionality, testing ensures that changes work correctly and have not caused unforeseen issues.

- **Confirmation testing**: After fixing a defect, the failed test cases (due to the defect) should be re-executed in the updated software version. The steps to reproduce the original failure should also be re-executed.
- **Regression testing**: Changes to one part of the code can affect other parts, even in different components or systems. Regression testing helps detect these unintended side effects.

Change-related testing (confirmation and regression testing) occurs at all test levels, especially in iterative and incremental development (e.g., Agile). Frequent changes in features, refactoring, or updates, as seen in IoT systems, increase the need for confirmation and regression testing. **Regression test suites** should be automated early to ensure thorough and efficient testing.

### 2.3.5 Test Types and Test Levels
Any test type (functional, non-functional, white-box, change-related) can be executed at any test level. Below are examples for a banking application across different test levels:

- **Functional tests**:
    - **Component testing**: Tests the component that calculates compound interest.
    - **Component integration testing**: Verifies how account data is passed from the UI to the business logic.
    - **System testing**: Tests how account holders apply for a line of credit.
    - **System integration testing**: Tests the external microservice used to check credit scores.
    - **Acceptance testing**: Validates the banker’s process for approving or declining credit applications.

- **Non-functional tests**:
    - **Component testing**: Measures CPU cycles required for complex interest calculations.
    - **Component integration testing**: Security tests for buffer overflow vulnerabilities.
    - **System testing**: Tests browser and mobile device compatibility.
    - **System integration testing**: Evaluates system robustness when the credit score microservice fails.
    - **Acceptance testing**: Assesses accessibility of the credit processing interface for users with disabilities.

- **White-box tests**:
    - **Component testing**: Ensures complete statement and decision coverage for financial calculation components.
    - **Component integration testing**: Tests how screens pass data to the business logic.
    - **System testing**: Covers sequences of web pages during a credit line application.
    - **System integration testing**: Tests all inquiry types sent to the credit score microservice.
    - **Acceptance testing**: Covers supported financial data file structures for bank-to-bank transfers.

- **Change-related tests**:
    - **Component testing**: Automated regression tests for each component, run within the continuous integration framework.
    - **Component integration testing**: Tests interface fixes in the code repository.
    - **System testing**: Re-executes tests for workflows when any screen in the workflow changes.
    - **System integration testing**: Daily re-execution of tests with the credit scoring microservice as part of continuous deployment.
    - **Acceptance testing**: Re-executes all previously failed tests after a defect fix.

While all test types don’t need to be represented at every level, applicable tests should be run at the earliest level possible.

### 2.4 Maintenance Testing
After deployment, software requires maintenance, either to fix defects found in production, add new functionality, or alter existing functionality. Maintenance also includes efforts to preserve or enhance non-functional quality characteristics of the system.
