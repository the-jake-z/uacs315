# October 7, 2015 - CS 315
## Sequence Diagram Lab

### Sequence Diagram

- Illustrate a sequence of actions occuring in a system.

- Consists of 3 elements
	- Objects
	- Life lines
	- Messages

- Used to Capture dynamic behavior
- Describe message flow
- Describe the structural flow

- Class diagrams describe the strucutre of instances. 
- Sequence diagram represents the behavior of an application.
- Depict dynamic, runtime behavior between objects (not an internal view).
- Sequence Diagrams introduce the notion of time
	- Sometimes abstracted to process.
	- Moves down the vertical

- Vertical Axis is time
- Objects (particpants) exchange messages in a behavior trace are shown across the top
- Every vertical dashed line is a "Life line".

- Special method sent to the object to denote object creation.
- an X to symbolize the end of life of an object.
	- In a garbage collected language no need to worry
	- In other languages you have to call the dispose method.

The use case description should have enough detail to define a logical sequence diagram.

### Message Flow

- Communication between objects can be
	- Synchronous, everything else stops until some message is returned (represented by closed triangle)
	- Asynchronous, execution continues without waiting for a return message. (represented by open triangle)
- Messages rely on the method definitions in the class diagram.
- Should be consisten with the class diagram.

Fragments

- alt alternative fragment in th
- ref reference another diagram
- sd surround an entire diagram for future references

Huseyin walked through the use-case example in class for the Deposit Funds Use-Case found in prior labs.


