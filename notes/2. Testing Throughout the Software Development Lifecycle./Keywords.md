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

