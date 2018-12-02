# Iteration 1: Establishing an overall System Structure

#### Step 2: Establish Iteration Goal by Selecting Drivers

The iteration goal is to establish an overall system structure

#### Step 3: Choose one or more elements of the System to Refine

#### Step 4: Choose One or More Design Concepts that Satisfy the Selected Drivers

| Design Decisions and Location                                | Rationale                                                    |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| Use the Web Applications reference architecture to structure the client part of the system | The three layers will support the system. The presentation layer can contain modules responsible for user interaction(CON-5). The data layer contains modules that handle data stored either locally or remotely (CON-6). |
| three-tier distributed deployment                            | Allows flexibility in regards to components residing in different tiers. Allows scalability as more tiers can be added. Adds security with firewalls between layers and security policies may be added to tiers.  Database can be stored in a layer separate from the application. |
|                                                              |                                                              |

#### Step 5: Instantiate Architectural Elements, Allocate Responsibilities, and Define Interfaces

#### Step 6: Sketch Views and Record Design Decisions 

#### Step 7: Perform Analysis of Current Design and Review Iteration Goal and Achievement of Design Purpose