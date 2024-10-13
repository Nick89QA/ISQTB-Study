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

### Walkthrough
- **Main purposes**: find defects, improve the software product, consider alternative implementations, evaluate conformance to standards and specifications
- **Possible additional purposes**: exchanging ideas about techniques or style variations, training of participants, achieving consensus
- **Individual preparation before the review meeting is optional**
- **Review meeting** is typically led by the author of the work product
- **Scribe** is mandatory
- **Use of checklists** is optional
- May take the form of scenarios, dry runs, or simulations
- Potential defect logs and review reports are produced
- May vary in practice from quite informal to very formal

### Technical Review
- **Main purposes**: gaining consensus, detecting potential defects
- **Possible further purposes**: evaluating quality and building confidence in the work product, generating new ideas, motivating and enabling authors to improve future work products, considering alternative implementations
- **Reviewers** should be technical peers of the author and technical experts in the same or other disciplines
- **Individual preparation** before the review meeting is required
- **Review meeting** is optional, ideally led by a trained facilitator (typically not the author)
- **Scribe** is mandatory, ideally not the author
- **Use of checklists** is optional
- Potential defect logs and review reports are produced

### Inspection
- **Main purposes**: detecting potential defects, evaluating quality and building confidence in the work product, preventing future similar defects through author learning and root cause analysis
- **Possible further purposes**: motivating and enabling authors to improve future work products and the software development process, achieving consensus
- **Follows a defined process** with formal documented outputs, based on rules and checklists
- **Uses clearly defined roles**, such as those specified in section 3.2.2 which are mandatory, and may include a dedicated reader (who reads the work product aloud often paraphrasing it during the review meeting)
- **Individual preparation** before the review meeting is required
- **Reviewers** are either peers of the author or experts in other disciplines relevant to the work product
- **Specified entry and exit criteria** are used
- **Scribe** is mandatory
- **Review meeting** is led by a trained facilitator (not the author)
- **Author** cannot act as the review leader, reader, or scribe
- Potential defect logs and review reports are produced
- **Metrics** are collected and used to improve the software development process, including the inspection process

### 3.2.4 Applying Review Techniques
There are several review techniques that can be applied during the individual review activity to uncover defects. These techniques can be used across the review types described above. The effectiveness of the techniques may differ depending on the type of review used.

#### Ad Hoc
- **Process**: Reviewers are provided with little or no guidance. They often read the work product sequentially, identifying and documenting issues as they encounter them.
- **Advantages**: Commonly used and needs little preparation.
- **Disadvantages**: Highly dependent on reviewer skills, may lead to duplicate issues being reported by different reviewers.

#### Checklist-based
- **Process**: Reviewers detect issues based on checklists distributed at review initiation. Checklists consist of questions derived from experience or previous defects.
- **Advantages**: Systematic coverage of typical defect types.
- **Disadvantages**: Reviewers should not be constrained to the checklist and should look for defects outside the checklist.

#### Scenarios and Dry Runs
- **Process**: Reviewers are provided with structured guidelines to perform dry runs on the work product based on expected usage.
- **Advantages**: Helps identify specific defect types based on usage scenarios.
- **Disadvantages**: Reviewers should not miss other defect types outside documented scenarios.

#### Perspective-based
- **Process**: Reviewers take on different stakeholder viewpoints (e.g., end user, tester, operations) to gain depth in reviewing.
- **Advantages**: Leads to more in-depth reviewing with fewer duplicated issues.
- **Additional**: Requires reviewers to attempt to generate the product they would derive from the work product under review (e.g., testers generate draft acceptance tests from requirements).
### Perspective-based
- **Process**: Reviewers evaluate the work product from different stakeholder viewpoints to see if all necessary information was included. Checklists are expected to be used.
- **Effectiveness**: Empirical studies show that perspective-based reading is the most effective general technique for reviewing requirements and technical work products.
- **Key Success Factor**: Including and weighing different stakeholder viewpoints appropriately, based on risks.
- **References**: Shul (2000) for details on perspective-based reading, Sauer (2000) for the effectiveness of different review techniques.

### Role-based
- **Process**: Reviewers evaluate the work product from the perspective of individual stakeholder roles (e.g., specific end user types like experienced, inexperienced, senior, child, or roles like user administrator, system administrator, performance tester, etc.).
- **Similarities**: Follows the same principles as perspective-based reading, focusing on individual stakeholder roles.

### 3.2.5 Success Factors for Reviews
To ensure a successful review, the right type of review and techniques must be used. Additional factors that influence the outcome of a review include:

#### Organizational Success Factors:
- Each review has **clear objectives**, defined during review planning, and used as measurable exit criteria.
- The selected **review types** are suitable to achieve the objectives and are appropriate for the type and level of software work products and participants.
- **Review techniques** used (e.g., checklist-based, role-based) are appropriate for effective defect identification in the work product.
- Any **checklists used** are up to date and address the main risks.
- **Large documents** are written and reviewed in small chunks to allow for early and frequent feedback on defects.
- Participants are given **adequate time to prepare**.
- Reviews are scheduled with **adequate notice**.
- **Management supports** the review process (e.g., by incorporating adequate time for review activities in project schedules).
- Reviews are integrated into the company's **quality** and/or **test policies**.
  People-related success factors for reviews include:
  • The right people are involved to meet the review objectives, for example, people with different skill sets or perspectives, who may use the document as a work input
  • Testers are seen as valued reviewers who contribute to the review and learn about the work product, which enables them to prepare more effective tests, and to prepare those tests earlier
  • Participants dedicate adequate time and attention to detail
  • Reviews are conducted on small chunks, so that reviewers do not lose concentration during
  individual review and/or the review meeting (when held)
  • Defects found are acknowledged, appreciated, and handled objectively
  • The meeting is well-managed, so that participants consider it a valuable use of their time
  • The review is conducted in an atmosphere of trust; the outcome will not be used for the evaluation of the participants
  • Participants avoid body language and behaviors that might indicate boredom, exasperation, or hostility to other participants
  • Adequate training is provided, especially for more formal review types such as inspections
  • A culture of learning and process improvement is promoted
  (See Gilb 1993, Wiegers 2002, and van Veenendaal 2004 for more on successful reviews.)