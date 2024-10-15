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