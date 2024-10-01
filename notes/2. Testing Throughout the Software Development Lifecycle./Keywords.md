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

