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