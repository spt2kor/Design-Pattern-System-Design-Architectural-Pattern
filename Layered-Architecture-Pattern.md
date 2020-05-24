Layered Architecture Pattern
http://posa1.blogspot.com/2008/05/layered-architecture-pattern.html

The Layered architectural pattern helps to structure applications that can be decomposed into groups of subtasks in which each group of subtasks Is at a particular level of abstraction.


Context:
Large system that requires decomposition.

The following scenarios are archetypes for the dynamic behavior of layered applications.

Scenario I : probably the best-known one. A client issues a request to Layer N. Since Layer N cannot cany out the request on its own, it calls the next Layer N -1 for supporting subtasks. Layer N -1 provides these, in the process sending further requests to Layer N -2, and so on until Layer 1 is reached. Here, the lowest-level services are finally performed. If necessary, replies to the different requests are passed back up from Layer 1 to Layer 2, from Layer 2 to Layer 3, and so on until the final reply arrives at Layer N.
Scenario II : illustrates bottom-up communication-a chain of actions starts at Layer 1, for example when a device driver detects input. The driver translates the input into an internal format and reports it to Layer 2, which starts interpreting it, and so on. In this way data moves up through the layers until it arrives at the highest layer. Whiletop-down information and control flow are often described as 'requests', bottom-up calls can be termed 'notifications'.
Scenario III : describes the situation where requests only travel through a subset of the layers. A top-level request may only go to the next lower level N -1 if this level can satisfy the request.
Scenario IV : describes a situation similar to Scenario III. An event is detected in Layer 1, but stops at Layer 3 instead of traveling all the way up to Layer N.
Scenario V : involves two stacks of N layers communicating with each other. This scenario is well-known from communication protocols where the stacks. are known as 'protocol stacks'.