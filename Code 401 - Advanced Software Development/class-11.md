# Event Driven Applications

ability of Javascript to raise events, monitor events, and perform operations in response to events occurring.

## Review, Research, and Discussion

1. Why is access control important?

   Access controls limit access to information and information processing systems. When implemented effectively, they mitigate the risk of information being accessed without the appropriate authorisation, unlawfully and the risk of a data breach

2. Describe an application that would need access control.

   Access management system.

3. What is a role used for?

   to facilitate administration of security in large organizations with hundreds of users and thousands of permissions.

4. Why is role based access control more scalable than discretionary or mandatory access control?

   better serves a company-wide security system with an overseeing administrator, grant write access to a specific file, but it cannot determine how a user might change the file

## Vocabulary Terms

| Word                      | Definition                                                                                                                                                                                     |
| ------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Authorization             | is the function of specifying access rights/privileges to resources, which is related to general information security and computer security, and to access control in particular               |
| Role Based Access Control | Role-based access control (RBAC) is a method of restricting network access based on the roles of individual users within an enterprise.                                                        |
| Capabilities              | A capability (known in some systems as a key) is a communicable, unforgeable token of authority. It refers to a value that references an object along with an associated set of access rights. |

## Preview

### Event Driven Programming

- a program is designed to respond to user engagement in various forms. It is known as a programming paradigm in which the flow of program execution is determined by “events.” Events are any user interaction, such as a click or key press, in response to prompt from the system.

For the most recognizable example of Event-Driven Programming for people at any level of programming skill, we’ll turn to our old friend The Web Browser.

Every time you interact with a webpage through it’s user interface, an event is happening. When you click a button a click event is triggered. When you press a key a keydown event is triggered. These events have associated functions that, when triggered, are executed to make a change to the user interface in some way.

### Node docs: events

- Class: EventEmitter
  - Event: 'newListener'
  - Event: 'removeListener'
