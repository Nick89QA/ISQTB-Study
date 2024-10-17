### Keywords:
- Black-box test technique
- Boundary value analysis
- Checklist-based testing
- Coverage
- Decision coverage
- Decision table testing
- Error guessing
- Equivalence partitioning
- Experience-based test technique
- Exploratory testing
- State transition testing
- Statement coverage
- Test technique
- Use case testing
- White-box test technique

---

### Learning Objectives for Test Techniques

#### 4.1 Categories of Test Techniques
- **FL-4.1.1 (K2)**: Explain the characteristics, commonalities, and differences between black-box test techniques, white-box test techniques, and experience-based test techniques.

#### 4.2 Black-box Test Techniques
- **FL-4.2.1 (K2)**: Explain error guessing.
- **FL-4.2.2 (K2)**: Explain exploratory testing.
- **FL-4.2.3 (K2)**: Explain checklist-based testing.
- **FL-4.2.4 (K3)**: Apply equivalence partitioning to derive test cases from given requirements.
- **FL-4.2.5 (K3)**: Apply boundary value analysis to derive test cases from given requirements.
- **FL-4.2.6 (K3)**: Apply decision table testing to derive test cases from given requirements.
- **FL-4.2.7 (K3)**: Apply state transition testing to derive test cases from given requirements.
- **FL-4.2.8 (K2)**: Explain how to derive test cases from a use case.

#### 4.3 White-box Test Techniques
- **FL-4.3.1 (K2)**: Explain statement coverage.
- **FL-4.3.2 (K2)**: Explain decision coverage.
- **FL-4.3.3 (K2)**: Explain the value of statement and decision coverage.

---

### 4.1 Categories of Test Techniques

The purpose of a test technique is to help in identifying test conditions, test cases, and test data. The choice of test techniques depends on several factors, including:
- Component or system complexity
- Regulatory standards
- Customer or contractual requirements
- Risk levels and types
- Available documentation
- Tester knowledge and skills
- Available tools
- Time and budget
- Software development lifecycle model
- Types of defects expected in the component or system

Some techniques are more applicable to certain situations and test levels, while others can be applied across all test levels. Testers often use a combination of test techniques to achieve the best results.

The use of test techniques can range from informal (little to no documentation) to formal. The appropriate level of formality depends on the testing context, including:
- Maturity of test and development processes
- Time constraints
- Safety or regulatory requirements
- The knowledge and skills of the people involved
- The software development lifecycle model

---

### 4.1.1 Categories of Test Techniques and Their Characteristics

In this syllabus, test techniques are classified as **black-box**, **white-box**, or **experience-based**.

#### Black-box Test Techniques:
- Also called behavioral or behavior-based techniques.
- Based on the analysis of the test basis (e.g., formal requirements, use cases, user stories, business processes).
- Applicable to both functional and non-functional testing.
- Focus on inputs and outputs without reference to the internal structure.

#### White-box Test Techniques:
- Also called structural or structure-based techniques.
- Based on the analysis of the architecture, detailed design, internal structure, or code.
- Focus on the structure and processing within the test object.

#### Experience-based Test Techniques:
- Leverage the experience of developers, testers, and users.
- Combined often with black-box and white-box techniques.
### Test Cases and Coverage
- Test cases may be used to detect gaps between the requirements and the implementation, as well as deviations from the requirements.
- Coverage is measured based on the items tested in the test basis and the technique applied to the test basis.

### Common Characteristics of White-box Test Techniques
- Test conditions, test cases, and test data are derived from a test basis that may include code, software architecture, detailed design, or any other structural information about the software.
- Coverage is measured based on the items tested within a selected structure (e.g., code or interfaces) and the technique applied.

### Common Characteristics of Experience-based Test Techniques
- Test conditions, test cases, and test data are derived from the knowledge and experience of testers, developers, users, and other stakeholders.
- This experience includes expected use of the software, its environment, likely defects, and the distribution of those defects.

The international standard (ISO/IEC/IEEE 29119-4) contains descriptions of test techniques and their corresponding coverage measures (see Craig 2002 and Copeland 2004 for more information on techniques).

---

## 4.2 Black-box Test Techniques

### 4.2.1 Equivalence Partitioning
- Equivalence partitioning divides data into partitions (also called equivalence classes) where all members of a partition are expected to be processed in the same way (see Kaner 2013 and Jorgensen 2014).
- There are **valid** and **invalid** equivalence partitions:
    - **Valid equivalence partition**: Contains values that should be accepted by the system.
    - **Invalid equivalence partition**: Contains values that should be rejected by the system.

#### Key Points:
- Partitions can apply to inputs, outputs, internal values, time-related values, and interface parameters.
- Partitions may be divided into sub-partitions if necessary.
- Each value must belong to one and only one equivalence partition.
- Invalid equivalence partitions should be tested individually to avoid masking defects.
- **Coverage** is measured as the number of tested partitions divided by the total number of partitions, expressed as a percentage.
- Equivalence partitioning is applicable at all test levels.

### 4.2.2 Boundary Value Analysis (BVA)
- BVA is an extension of equivalence partitioning that focuses on **numeric or sequential data**.
- Boundary values are the minimum and maximum values of a partition (see Beizer 1990).

#### Example:
- If a field accepts integers from 1 to 5, the partitions are:
    - Invalid (too low): 0
    - Valid: 1–5
    - Invalid (too high): 6
- For 100% coverage, test cases must cover both boundaries (e.g., 0, 1, 5, 6).

#### Variations:
- Some techniques use three boundary values: before, at, and just over the boundary.

#### Application:
- BVA applies to testing ranges (numbers, dates, times) and can be used at all test levels.
- **Boundary coverage** is measured as the number of boundary values tested divided by the total number of boundary values.

### 4.2.3 Decision Table Testing
- Decision tables are useful for recording complex business rules.
- Testers identify conditions (inputs) and actions (outputs), forming the rows of the table.
- Columns correspond to decision rules, with each column defining a unique combination of conditions resulting in specific actions.

#### Notation:
- **For conditions**:
    - Y = condition is true (may also be T or 1)
    - N = condition is false (may also be F or 0)
    - — = condition doesn’t matter (N/A)
- **For actions**:
    - X = action should occur (may also be Y, T, or 1)

- **Blank** means the action should not occur (may also be shown as —, N, F, or 0).
- A **full decision table** includes enough columns (test cases) to cover every combination of conditions. Reducing columns by removing impossible combinations can decrease the number of test cases. For more information on collapsing decision tables, see ISTQB-CTAL-AT.

### Coverage for Decision Table Testing
- The common minimum coverage standard is to have at least one test case per decision rule. This typically covers all combinations of conditions.
- **Coverage** is measured as the number of decision rules tested by at least one test case, divided by the total number of decision rules, expressed as a percentage.

#### Strength of Decision Table Testing:
- Helps identify important combinations of conditions that might otherwise be overlooked.
- Assists in finding gaps in requirements.
- Can be applied at any test level where the behavior depends on a combination of conditions.

---

### 4.2.4 State Transition Testing
- In **state transition testing**, components or systems respond differently to events depending on current conditions or previous history (events since the system was initialized).
- **States** summarize the previous history, and **state transition diagrams** show possible software states, transitions between states, and actions triggered by events (e.g., user inputs).
- The same event can cause different transitions based on the current state.

#### Key Elements:
- **State Transition Table**: Shows valid and potentially invalid transitions between states, the events that trigger them, and the resulting actions.
- Tests can be designed to:
    - Cover typical sequences of states
    - Exercise all states and transitions
    - Test specific sequences of transitions or invalid transitions.

#### Application:
- Used in **menu-based applications** and widely within the **embedded software** industry.
- Suitable for modeling business scenarios with specific states or testing screen navigation.
- **Coverage** is measured by the number of identified states or transitions tested, divided by the total number of states or transitions in the test object.

---

### 4.2.5 Use Case Testing
- **Use case testing** derives tests from **use cases**, which define interactions with software items. These incorporate software functional requirements.
- **Actors** (users, external hardware, or other components) and **subjects** (the system to which the use case applies) are involved in the use cases.

#### Key Elements:
- A use case specifies the behavior a subject performs with one or more actors.
- Descriptions of use cases include **preconditions**, **postconditions**, interactions, and **activities**. Natural language descriptions may also be used.
- **Interactions** between actors and the subject can result in changes to the subject’s state.
- Graphical representations such as **workflows**, **activity diagrams**, or **business process models** may be used.

A use case can include possible variations of its basic behavior, such as **exceptional behavior** and **error handling** (e.g., system responses to programming, application, or communication errors). Tests are designed to exercise basic, alternative, and exceptional behaviors, including error handling. **Coverage** is measured by the number of use case behaviors tested, divided by the total number of use case behaviors, usually expressed as a percentage.

For more information on coverage criteria for use case testing, see ISTQB-CTAL-AT.

---

### 4.3 White-box Test Techniques

White-box testing focuses on the internal structure of the test object and is applicable at all test levels. The two white-box techniques discussed below are most common at the **component test** level.

For more advanced white-box techniques used in safety-critical environments, see ISTQB-CTAL-TTA.

#### 4.3.1 Statement Testing and Coverage
- **Statement testing** exercises the executable statements in the code.
- **Coverage** is measured as the number of statements executed divided by the total number of executable statements in the test object, expressed as a percentage.

#### 4.3.2 Decision Testing and Coverage
- **Decision testing** focuses on decision points in the code and tests the code executed based on decision outcomes.
- Test cases are designed to follow control flows from decision points (e.g., IF statements require test cases for both true and false outcomes; CASE statements need test cases for all possible outcomes, including defaults).
- **Coverage** is measured as the number of decision outcomes executed divided by the total number of decision outcomes in the test object, expressed as a percentage.

#### 4.3.3 The Value of Statement and Decision Testing
- Achieving 100% **statement coverage** ensures all executable statements are tested, but not all decision logic.
- 100% **decision coverage** ensures all decision outcomes (true and false) are tested. Achieving 100% decision coverage also guarantees 100% statement coverage, but not vice versa.
- **Statement coverage** helps find defects in unexecuted code, while **decision coverage** helps identify issues in logic that tests may miss.

---

### 4.4 Experience-based Test Techniques
Experience-based test techniques derive test cases from the **tester’s skills**, **intuition**, and **experience** with similar systems. These techniques may uncover test cases that systematic methods might overlook. The effectiveness and coverage of experience-based techniques can vary widely depending on the tester’s background. **Coverage** can be difficult to assess and may not be easily measurable.

Commonly used experience-based techniques are discussed in the following sections.

### 4.4.1 Error Guessing
**Error guessing** is a technique used to anticipate errors, defects, and failures based on the tester’s knowledge and experience. This can include:
- How the application has behaved in the past
- Common types of errors that tend to be made
- Failures encountered in other applications

A methodical approach to error guessing involves creating a **list of possible errors**, defects, and failures, then designing tests to expose those failures and the underlying defects. These lists can be built from:
- Personal experience
- Historical defect and failure data
- Common knowledge about why software tends to fail.

### 4.4.2 Exploratory Testing
**Exploratory testing** involves designing, executing, logging, and evaluating tests dynamically during test execution. The test results help testers learn more about the system and identify areas that may need further testing.

This approach is often used when:
- Specifications are incomplete or unclear
- There is significant time pressure
- As a complement to more formal testing techniques

Exploratory testing can be structured using **session-based testing**, where testing is conducted within a defined time-box. Testers follow a **test charter** that outlines objectives and may document their steps and findings using **test session sheets**.

Exploratory testing is commonly associated with **reactive test strategies** (see section 5.2.2) and can include black-box, white-box, and experience-based techniques.

### 4.4.3 Checklist-based Testing
In **checklist-based testing**, testers create and execute tests based on conditions found in a **checklist**. These checklists can be newly created or expanded based on experience, user requirements, or common software failures. Existing checklists may also be used without modification.

Checklists can support both **functional and non-functional testing**, providing guidelines and a degree of consistency when detailed test cases are unavailable. While high-level, checklists allow flexibility in testing, which can increase coverage but reduce repeatability.