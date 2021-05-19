# Data Modeling

reading material, code samples, and some additional resources that support today’s topic and the upcoming lecture.

## Review, Research, and Discussion

1. Name 3 advantages to Test Driven Development.

   - Better program design and higher code quality.
   - Detailed project documentation.
   - Code flexibility and easier maintenance.

2. In what case would you need to use `beforeEach()` or `afterEach()` in a test suite?

   - in case that the tests consumes a particular global state for each test, for example, resetting test data in database beafore each test run.

3. What is one downside of Test Driven Developmen?

   - `slow process`: you simply need an extended duration of your time for straightforward implementations. you would like to believe the interfaces, write the test code, and run the tests before you’ll finally start writing the code.

4. What’s the primary difference between ES6 Classes and Constructor/Prototype Classes?

   - a class defines a type which can be instantiated at runtime, whereas a prototype is itself an object instance.

5. Why REST?
   - REST aims to make caching easier. Since the server is stateless and each request can be processed individually, GET requests should usually return the same response regardless of previous ones and the session. This makes the GET requests easily cacheable and browsers usually treat them as such.

## Vocabulary terms

|             **Term**              |                                                                                                    **Definition **                                                                                                    |
| :-------------------------------: | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
|      Functional programming       |                           way of thinking about software construction by creating pure functions. It avoid concepts of shared state, mutable data observed in Object Oriented Programming.                            |
| object-oriented programming (OOP) |      is a computer programming model that organizes software design around data, or objects, rather than functions and logic. An object can be defined as a data field that has unique attributes and behavior.       |
|              Classes              | template for creating objects. They encapsulate data with code to work on that data. Classes in JS are built on prototypes but also have some syntax and semantics that are not shared with ES5 class-like semantics. |
|              `super`              |                                                                     The super keyword is used to access and call functions on an object's parent.                                                                     |
|              `this`               |                        A function's this keyword behaves a little differently in JavaScript compared to other languages. It also has some differences between strict mode and non-strict mode.                        |
|   Test Driven Development (TDD)   |                           Test-driven development (TDD) is a software development process relying on software requirements being converted to test cases before software is fully developed                           |
|               Jest                |                                                           Jest is a JavaScript testing framework designed to ensure correctness of any JavaScript codebase.                                                           |
|    Continuous Integration (CI)    |                                                          is the practice of merging all developers' working copies to a shared mainline several times a day                                                           |
|               REST                |                                                         Representational state transfer (REST) is a software architectural style which uses a subset of HTTP.                                                         |
|            Data Model             |                     A data model (or datamodel) is an abstract model that organizes elements of data and standardizes how they relate to one another and to the properties of real-world entities                     |
