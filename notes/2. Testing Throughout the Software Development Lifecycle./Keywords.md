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
Page 29
