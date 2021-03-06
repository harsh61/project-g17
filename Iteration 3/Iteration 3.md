# Iteration 3: Addressing Quality Attribute Scenario Driver (QA-)

In this iteration we want to refine previously created structures to address the remaining drivers. Tactics, Deployment patterns and Architectural patterns will be used.

The driver for this iteration will be QA-2 security:   All data kept private to relevant users, data visibility and modifiability up to discretion of user / lecturers / administrators.



#### Step 2: Establish Iteration Goal by Selecting Drivers

The driver for this iteration will be QA-2 security:   All data kept private to relevant users, data visibility and modifiability up to discretion of user / lecturers / administrators.

The remaining QA scenarios and remaining drivers will also be considered, as this will be the final iteration and we want to address the remaining drivers.

#### Step 3: Choose one or more elements of the System to Refine

The elements being refined are the application server and the database server.

#### Step 4: Choose One or More Design Concepts that Satisfy the Selected Drivers

| Design Decisions and Location                                | Rationale and Assumptions                                    |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| Introduce the security tactic to resist attacks This can be done by using the Spring Security framework to manage authorization and authentication | The rationale behind this decision is that it supports the driver QA-2. This spring security framework can be implemented as part of the application server and database server. It allows for the managing of authorization and authentication. Alternatives considered include: Ad hoc code which was discarded because it would take a lot more resources to develop an authentication system from scratch as opposed to implementing a frame work. |
| Use the interoperability tactic                              | The discover service tactic can be used to address CON-3. It is used to search for locations on the service. |



#### Step 5: Instantiate Architectural Elements, Allocate Responsibilities, and Define Interfaces

| Design Decisions and Locations                              | Rationale                                                    |
| ----------------------------------------------------------- | ------------------------------------------------------------ |
| The Spring security framework is added as a component       | this addresses QA-2. It will allow for authentication and authorization of the users attempting to access data. |
| A discover service component is added in the services layer | When a user is making a request they can use the discover service to search for services. Allowing them to reach content within 3 clicks. |
|                                                             |                                                              |



#### Step 6: Sketch Views and Record Design Decisions 

![1544061687351](C:\Users\100462146\AppData\Roaming\Typora\typora-user-images\1544061687351.png)



#### 

| Element          | Responsibility                                               |
| ---------------- | ------------------------------------------------------------ |
| Security Manager | The security manager module is implemented using Spring Security. It handles authentication of users and keeps data private to relevant users. |
| Discover Service | This module allows users to locate a service by searching a known directory. |
|                  |                                                              |

#### 

#### Step 7: Perform Analysis of Current Design and Review Iteration Goal and Achievement of Design Purpose

| Not Addressed | Partially Addressed | Completely Addressed | Design Decisions Made During the Iteration                   |
| ------------- | ------------------- | -------------------- | ------------------------------------------------------------ |
|               |                     | QA-2                 | Security Manager module implemented                          |
|               |                     | QA-3                 | Discover service tactic implemtented                         |
|               | QA-4                |                      | The use case related to this QA has been identified.         |
|               |                     | CON-1                | Security Manager module implemented                          |
|               | CON-3               |                      | No relevant decisions made                                   |
|               | CON-4               |                      | The data abstraction module for secondary systems has been identified. |
|               | CON-5               |                      | The data abstraction module for secondary systems has been identified. |