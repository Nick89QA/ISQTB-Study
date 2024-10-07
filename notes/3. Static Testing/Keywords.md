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