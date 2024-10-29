# 6. Tool Support for Testing

## Keywords
- **Data-Driven Testing**: A testing approach where test data is separated from test scripts, allowing for multiple data sets to be used with a single test script.
- **Keyword-Driven Testing**: A testing technique that uses keywords to represent actions in test scripts, making tests more readable and maintainable.
- **Test Automation**: The use of software to perform testing tasks automatically.
- **Test Execution Tool**: Software used to execute tests, typically automating the running of test scripts.
- **Test Management Tool**: Software used for managing test cases, planning test activities, tracking test progress, and managing defects.

## Learning Objectives for Test Tools
### 6.1 Test Tool Considerations

#### Objectives
- **FL-6.1.1 (K1)**: Identify the main principles for selecting a tool.
- **FL-6.1.2 (K1)**: Recall the objectives for using pilot projects to introduce tools.
- **FL-6.1.3 (K1)**: Identify the success factors for evaluation, implementation, deployment, and ongoing support of test tools in an organization.

#### Test Tool Types and Benefits
- **FL-6.2.1 (K2)**: Classify test tools according to their purpose and the test activities they support.
- **FL-6.2.2 (K1)**: Identify benefits and risks of test automation.
- **FL-6.2.3 (K1)**: Remember special considerations for test execution and test management tools.

### 6.2 Effective Use of Tools
This section emphasizes understanding the principles, classification, and effective usage of test tools, along with their potential benefits and risks.

## 6.1 Test Tool Considerations

Test tools support a wide range of testing activities. These tools include:
- **Direct Testing Tools**: Such as test execution tools and test data preparation tools.
- **Management Tools**: For managing requirements, test cases, test procedures, automated scripts, test results, test data, defects, and for reporting and monitoring test execution.
- **Analysis and Evaluation Tools**: For reviewing data and providing insights.
- **Supporting Tools**: Any tool that assists in testing, even a spreadsheet for tracking test data or results.

### 6.1.1 Test Tool Classification

Test tools are classified based on their purpose, activity support, pricing, licensing, and technology. They may be designed to:
- **Automate Repetitive Tasks**: Reducing the resources required for tasks like regression testing.
- **Support Manual Testing Activities**: Improving manual processes throughout the test lifecycle.
- **Enhance Testing Quality**: By ensuring consistency and defect reproducibility.
- **Perform Non-Manual Tests**: Allowing for testing scenarios that are too resource-intensive to perform manually, like large-scale performance testing.
- **Increase Testing Reliability**: For example, automating data comparisons or simulating behavior in complex environments.

#### Tool Classifications
1. **Purpose-Based Classification**: Tools may serve multiple purposes but are classified under the activity they most support.
2. **Integrated Suites**: Tool providers often offer integrated suites designed to work seamlessly together.
3. **Intrusiveness**: Some tools may influence test outcomes, known as the *probe effect*. For example, a performance testing tool may alter response times by adding instructions to the application being tested.
4. **Developer-Oriented Tools**: Some tools, like those for component and integration testing, are more suited for developer use and are marked with “(D)” when listed.

#### Management Tools for Testing and Testware
These tools apply to test management across the software development lifecycle:
- **Test Management Tools**: Provide oversight of test activities and results.
- **Application Lifecycle Management (ALM) Tools**: Manage the software lifecycle from planning through testing to deployment.
- **Requirements Management Tools**: Aid in traceability between requirements and test cases.
- **Defect Management Tools**: Track and manage defects from detection through resolution.