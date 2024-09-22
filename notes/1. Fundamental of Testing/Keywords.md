# Keywords
- coverage
- debugging
- defect
- error
- failure
- quality
- quality assurance
- root cause
- test analysis
- test basis
- test case
- test completion
- test condition
- test control
- test data
- test design
- test execution
- test implementation
- test monitoring
- test object
- test objective
- test oracle
- test planning
- test procedure
- test process
- test suite
- testing
- testware
- traceability
- validation
- verification

# Learning Objectives for Fundamentals of Testing

## 1.1 What is Testing?

- **FL-1.1.1 (K1)**: Identify typical objectives of testing.
- **FL-1.1.2 (K2)**: Differentiate testing from debugging.

## 1.2 Why is Testing Necessary?

- **FL-1.2.1 (K2)**: Give examples of why testing is necessary.
- **FL-1.2.2 (K2)**: Describe the relationship between testing and quality assurance and give examples of how testing contributes to higher quality.
- **FL-1.2.3 (K2)**: Distinguish between error, defect, and failure.
- **FL-1.2.4 (K2)**: Distinguish between the root cause of a defect and its effects.

## 1.3 Seven Testing Principles

- **FL-1.3.1 (K2)**: Explain the seven testing principles.

## 1.4 Test Process

- **FL-1.4.1 (K2)**: Explain the impact of context on the test process.
- **FL-1.4.2 (K2)**: Describe the test activities and respective tasks within the test process.
- **FL-1.4.3 (K2)**: Differentiate the work products that support the test process.
- **FL-1.4.4 (K2)**: Explain the value of maintaining traceability between the test basis and test work products.

## 1.5 The Psychology of Testing

- **FL-1.5.1 (K1)**: Identify the psychological factors that influence the success of testing.
- **FL-1.5.2 (K2)**: Explain the difference between the mindset required for test activities and the mindset required for development activities.

# 1.1 What is Testing?

Software systems are an integral part of life, from business applications (e.g., banking) to consumer products (e.g., cars). Most people have had an experience with software that did not work as expected. Software that does not work correctly can lead to many problems, including loss of money, time, or business reputation, and even injury or death. Software testing is a way to assess the quality of the software and to reduce the risk of software failure in operation.

A common misperception of testing is that it only consists of running tests, i.e., executing the software and checking the results. As described in section 1.4, software testing is a process that includes many different activities; test execution (including checking of results) is only one of these activities. The test process also includes activities such as test planning, analyzing, designing, and implementing tests, reporting test progress and results, and evaluating the quality of a test object.

Some testing involves the execution of the component or system being tested; such testing is called **dynamic testing**. Other testing does not involve the execution of the component or system being tested; such testing is called **static testing**. Testing also includes reviewing work products such as requirements, user stories, and source code.

Another common misperception of testing is that it focuses entirely on **verification** of requirements, user stories, or other specifications. While testing does involve checking whether the system meets specified requirements, it also involves **validation**, which is checking whether the system will meet user and other stakeholder needs in its operational environment(s).

Test activities are organized and carried out differently in different lifecycles (see section 2.1).

## 1.1.1 Typical Objectives of Testing

For any given project, the objectives of testing may include:

- To prevent defects by evaluating work products such as requirements, user stories, design, and code.
- To verify whether all specified requirements have been fulfilled.
- To check whether the test object is complete and validate if it works as the users and other stakeholders expect.
- To build confidence in the level of quality of the test object.
- To find defects and failures by reducing the level of risk of inadequate software quality.
- To provide sufficient information to stakeholders to allow them to make informed decisions, especially regarding the level of quality of the test object.
- To comply with contractual, legal, or regulatory requirements or standards, and/or to verify the test object’s compliance with such requirements or standards.

The objectives of testing can vary, depending upon the context of the component or system being tested, the test level, and the software development lifecycle model. These differences may include, for example:

- During component testing, one objective may be to find as many failures as possible so that the underlying defects are identified and fixed early. Another objective may be to increase code coverage of the component tests.
- During acceptance testing, one objective may be to confirm that the system works as expected and satisfies requirements. Another objective of this testing may be to give information to stakeholders about the risk of releasing the system at a given time.

## 1.1.2 Testing and Debugging

Testing and debugging are different. Executing tests can show failures that are caused by defects in the software. Debugging is the development activity that finds, analyzes, and fixes such defects. Subsequent confirmation testing checks whether the fixes resolved the defects.

In some cases, testers are responsible for the initial test and the final confirmation test, while developers do the debugging, associated component, and component integration testing. However, in Agile development and in some other software development lifecycles, testers may be involved in debugging and component testing.
