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

## ISO standard (ISO/IEC/IEEE 29119-1) has further information about software testing concepts.

---

## 1.2 Why is Testing Necessary?

Rigorous testing of components and systems, and their associated documentation, can help reduce the risk of failures occurring during operation. When defects are detected, and subsequently fixed, this contributes to the quality of the components or systems. In addition, software testing may also be required to meet contractual or legal requirements or industry-specific standards.

---

### 1.2.1 Testing’s Contributions to Success

Throughout the history of computing, it is quite common for software and systems to be delivered into operation and, due to the presence of defects, to subsequently cause failures or otherwise not meet the stakeholders’ needs. However, using appropriate test techniques can reduce the frequency of such problematic deliveries, when those techniques are applied with the appropriate level of test expertise, in the appropriate test levels, and at the appropriate points in the software development lifecycle. Examples include:

- Having testers involved in requirements reviews or user story refinement could detect defects in these work products. The identification and removal of requirements defects reduces the risk of incorrect or untestable features being developed.
- Having testers work closely with system designers while the system is being designed can increase each party’s understanding of the design and how to test it. This increased understanding can reduce the risk of fundamental design defects and enable tests to be identified at an early stage.
- Having testers work closely with developers while the code is under development can increase each party’s understanding of the code and how to test it. This increased understanding can reduce the risk of defects within the code and the tests.
- Having testers verify and validate the software prior to release can detect failures that might otherwise have been missed, and support the process of removing the defects that caused the failures (i.e., debugging). This increases the likelihood that the software meets stakeholder needs and satisfies requirements.

In addition to these examples, the achievement of defined test objectives (see section 1.1.1) contributes to overall software development and maintenance success.

---

### 1.2.2 Quality Assurance and Testing

While people often use the phrase quality assurance (or just QA) to refer to testing, quality assurance and testing are not the same, but they are related. A larger concept, quality management, ties them together. Quality management includes all activities that direct and control an organization with regard to quality. Among other activities, quality management includes both quality assurance and quality control. Quality assurance is typically focused on adherence to proper processes, in order to provide confidence that the appropriate levels of quality will be achieved. When processes are carried out properly, the work products created by those processes are generally of higher quality, which contributes to defect prevention. In addition, the use of root cause analysis to detect and remove the causes of defects, along with the proper application of the findings of retrospective meetings to improve processes, are important for effective quality assurance.

Quality control involves various activities, including test activities, that support the achievement of appropriate levels of quality. Test activities are part of the overall software development or maintenance process. Since quality assurance is concerned with the proper execution of the entire process, quality assurance supports proper testing. As described in sections 1.1.1 and 1.2.1, testing contributes to the achievement of quality in a variety of ways.

---

### 1.2.3 Errors, Defects, and Failures

A person can make an error (mistake), which can lead to the introduction of a defect (fault or bug) in the software code or in some other related work product. An error that leads to the introduction of a defect in one work product can trigger an error that leads to the introduction of a defect in a related work product. For example, a requirements elicitation error can lead to a requirements defect, which then results in a programming error that leads to a defect in the code.

If a defect in the code is executed, this may cause a failure, but not necessarily in all circumstances. For example, some defects require very specific inputs or preconditions to trigger a failure, which may occur rarely or never.

Errors may occur for many reasons, such as:

- Time pressure
- Human fallibility
- Inexperienced or insufficiently skilled project participants
- Miscommunication between project participants, including miscommunication about requirements and design
- Complexity of the code, design, architecture, the underlying problem to be solved, and/or the technologies used
- Misunderstandings about intra-system and inter-system interfaces, especially when such intra-system and inter-system interactions are large in number
- New, unfamiliar technologies

In addition to failures caused due to defects in the code, failures can also be caused by environmental conditions. For example, radiation, electromagnetic fields, and pollution can cause defects in firmware or influence the execution of software by changing hardware conditions.
Page 15
