**Keywords**  
Ad hoc review, checklist-based review, dynamic testing, formal review, informal review, inspection, perspective-based reading, review, role-based review, scenario-based review, static analysis, static testing, technical review, walkthrough

---

## 3.1 Static Testing Basics

### FL-3.1.1
(K1) Recognize types of software work product that can be examined by the different static testing techniques.

### FL-3.1.2
(K2) Use examples to describe the value of static testing.

### FL-3.1.3
(K2) Explain the difference between static and dynamic techniques, considering objectives, types of defects to be identified, and the role of these techniques within the software lifecycle.

---

### 3.1 Static Testing Overview

In contrast to dynamic testing, which requires the execution of software, static testing involves manual examination of work products (e.g., reviews) or tool-driven analysis (e.g., static analysis). These methods help assess the quality of work products without executing them. Static analysis is often critical in safety-critical systems and is also widely used in security testing and automated build processes (e.g., in Agile).

---

### 3.1.1 Work Products for Static Testing

Static testing can be applied to a wide range of work products, including:
- Specifications (business, functional, security requirements)
- Epics, user stories, acceptance criteria
- Architecture and design documents
- Code
- Testware (test plans, test cases, scripts)
- User guides, web pages, contracts
- Project plans, schedules, and budgets
- Models (e.g., activity diagrams for Model-Based Testing)

Static analysis can be applied to formalized work products (code, models) and even to natural language products (e.g., checking requirements for readability, spelling).

---

### 3.1.2 Benefits of Static Testing

Static testing provides numerous benefits:
- Early detection of defects (before dynamic testing)
- Cheaper defect fixes (especially when caught early)
- Identifying defects not easily found through dynamic testing
- Preventing defects by finding issues in requirements and design (e.g., ambiguities, contradictions)
- Improving productivity and maintainability of code
- Reducing cost and time in development and testing
- Improving communication within the team through reviews

---

### 3.1.3 Differences Between Static and Dynamic Testing

Both static and dynamic testing aim to assess work product quality and detect defects, but they achieve this differently:
- Static testing finds defects in the work product directly, while dynamic testing finds failures caused by defects during software execution.
- Static testing can detect defects that might never cause failures during dynamic tests (e.g., unreachable code).
- Static testing improves internal quality (consistency, structure) of work products, while dynamic testing focuses on externally visible behavior.

Types of defects found more easily through static testing include:
- Requirement defects (e.g., inconsistencies, ambiguities)
- Design defects (e.g., inefficient algorithms, high coupling)
- Coding defects (e.g., unused variables, unreachable code)
- Deviations from standards
- Security vulnerabilities (e.g., buffer overflows)
- Gaps in traceability or coverage of test bases

Additionally, maintainability defects (e.g., poor modularization) are primarily found via static testing.

---

## 3.2 Review Process

### FL-3.2.1
(K2) Summarize the activities of the work product review process.

### FL-3.2.2
(K1) Recognize the different roles and responsibilities in a formal review.

### FL-3.2.3
(K2) Explain the differences between different review types: informal review, walkthrough, technical review, and inspection.

### FL-3.2.4
(K3) Apply a review technique to a work product to find defects.

### FL-3.2.5
(K2) Explain the factors that contribute to a successful review.

## 3.1 Static Testing Basics

In contrast to **dynamic testing**, which requires software execution, **static testing** relies on the manual examination of work products (e.g., reviews) or tool-driven evaluation of code or other work products (e.g., static analysis). Static testing evaluates the code or work product without execution.

**Static analysis** is crucial for **safety-critical systems** (e.g., aviation, medical, nuclear software) and is also essential in other contexts, like security testing. It's commonly used in **Agile**, **continuous delivery**, and **continuous deployment** processes.

---

### 3.1.1 Work Products That Can Be Examined by Static Testing

Static testing (reviews and/or static analysis) can be applied to nearly any work product, including:
- **Specifications** (business, functional, security requirements)
- **Epics, user stories, and acceptance criteria**
- **Architecture and design specifications**
- **Code**
- **Testware** (test plans, test cases, test procedures, automated test scripts)
- **User guides**
- **Web pages**
- **Contracts, project plans, schedules, and budgets**
- **Configuration and infrastructure setup**
- **Models** (e.g., activity diagrams for Model-Based Testing)

**Reviews** are applicable to any product that participants can read and understand. **Static analysis** is most efficient for formal structures (e.g., code, models) but can also be applied to natural language products (e.g., requirements checking for spelling, grammar, and readability).

---

### 3.1.2 Benefits of Static Testing

Static testing provides multiple benefits when applied early in the software development lifecycle, allowing early detection of defects before dynamic testing. This approach results in cost-effective defect removal, especially compared to the cost of fixing defects found later in the lifecycle (e.g., post-deployment).

Benefits include:
- Detecting defects **before dynamic test execution**
- Identifying defects **not easily found by dynamic testing**
- **Preventing defects** in design or coding (e.g., inconsistencies, ambiguities, inaccuracies)
- Increasing development **productivity** and code maintainability
- Reducing **development** and **testing** cost and time
- Lowering **total cost of quality** over the software’s lifecycle
- Improving team communication during review processes

---

### 3.1.3 Differences Between Static and Dynamic Testing

Static and dynamic testing share objectives (e.g., quality assessment, early defect detection), but they uncover different types of defects.

#### Key Differences:
- **Static testing** finds defects directly in work products (e.g., unexecuted code).
- **Dynamic testing** identifies failures caused by defects during software execution.
- Static testing is better at finding defects in rarely exercised or hard-to-reach paths.
- Static testing improves the **internal quality** of work products, whereas dynamic testing focuses on **externally visible behavior**.

#### Defects Found by Static Testing:
- **Requirement defects** (inconsistencies, ambiguities, omissions)
- **Design defects** (inefficient algorithms, high coupling, low cohesion)
- **Coding defects** (undefined variables, unreachable code, duplicate code)
- **Deviations from standards** (non-adherence to coding standards)
- **Interface specification errors** (e.g., mismatched units between systems)
- **Security vulnerabilities** (e.g., buffer overflows)
- **Gaps or inaccuracies in test basis traceability or coverage** (e.g., missing tests for an acceptance criterion)

Moreover, most types of **maintainability defects** can only be found through static testing, such as:
- **Improper modularization**
- **Poor reusability of components**
- **Code that is difficult to analyze or modify** without introducing new defects

## 3.2 Review Process

Reviews can range from **informal** to **formal**:
- **Informal reviews**: No defined process, no formal documented output.
- **Formal reviews**: Include team participation, documented results, and procedures for conducting the review.

### 3.2.1 Work Product Review Process

The review process consists of the following activities:

#### 1. Planning
- Defining scope, including the purpose, documents to be reviewed, and quality characteristics to evaluate.
- Estimating effort and timeframe.
- Identifying review characteristics (review type, roles, activities, and checklists).
- Selecting participants and assigning roles.
- Defining entry and exit criteria (for formal reviews like inspections).
- Ensuring entry criteria are met (in formal reviews).

#### 2. Initiate Review
- Distributing the work product and related materials (e.g., checklists, issue log forms).
- Explaining the scope, objectives, process, roles, and materials to participants.
- Answering participant questions about the review.

#### 3. Individual Review (Preparation)
- Reviewing the work product individually.
- Noting potential defects, recommendations, and questions.

#### 4. Issue Communication and Analysis
- Communicating potential defects (e.g., in a review meeting).
- Analyzing defects, assigning ownership and status.
- Evaluating and documenting quality characteristics.
- Evaluating the review findings against the exit criteria to make a review decision (reject; major changes needed; accept, possibly with minor changes)
### 3.2.2 Roles and Responsibilities in a Formal Review

- **Author**
    - Creates the work product under review.
    - Fixes defects in the work product (if necessary).

- **Management**
    - Responsible for review planning.
    - Decides on the execution of reviews.
    - Assigns staff, budget, and time.
    - Monitors ongoing cost-effectiveness.
    - Executes control decisions in the event of inadequate outcomes.

- **Facilitator (Moderator)**
    - Ensures effective running of review meetings (when held).
    - Mediates between different points of view if necessary.
    - The success of the review often depends on this role.

- **Review Leader**
    - Takes overall responsibility for the review.
    - Decides who will be involved and organizes when and where it will take place.

- **Reviewers**
    - May be subject matter experts, project team members, stakeholders, or individuals with specific technical or business backgrounds.
    - Identify potential defects in the work product under review.
    - May represent different perspectives (e.g., tester, developer, user, operator, business analyst, usability expert).

- **Scribe (Recorder)**
    - Collates potential defects found during the individual review activity.
    - Records new potential defects, open points, and decisions from the review meeting (when held).

In some review types, one person may play more than one role, and the actions associated with each role may vary. With the use of tools to support the review process, the need for a scribe is often eliminated. Further details are available in ISO standard (ISO/IEC 20246).

### 3.2.3 Review Types

Although reviews can be used for various purposes, one of the main objectives is to uncover defects. All review types can aid in defect detection, and the selected review type should be based on the needs of the project, available resources, product type and risks, business domain, and company culture, among other selection criteria.

A single work product may be the subject of more than one type of review. If more than one type of review is used, the order may vary. For example, an informal review may be carried out before a technical review, to ensure the work product is ready for a technical review.

The types of reviews described below can be done as peer reviews, i.e., done by colleagues qualified to do the same work. The types of defects found in a review vary, depending especially on the work product being reviewed. (See section 3.1.3 for examples of defects that can be found by reviews in different work products, and Gilb 1993 for information on formal inspections).

#### Informal Review (e.g., buddy check, pairing, pair review)
- **Main purpose**: detecting potential defects
- **Possible additional purposes**: generating new ideas or solutions, quickly solving minor problems
- **Not based on a formal (documented) process**
- **May not involve a review meeting**
- **May be performed by a colleague of the author (buddy check) or by more people**
- **Results may be documented**
- **Varies in usefulness depending on the reviewers**
- **Use of checklists is optional**
- **Very commonly used in Agile development**