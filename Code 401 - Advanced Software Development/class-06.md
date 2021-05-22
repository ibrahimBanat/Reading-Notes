# Authentication

reading material, code samples, and some additional resources that support today’s topic and the upcoming lecture.

## Review, Research, and Discussion

1. Explain what a “Singleton” is (in Computer Science terms).

   - design pattern comes under creational pattern as this pattern provides one of the best ways to create an object. This pattern involves a single class which is responsible to create an object while making sure that only single object gets created.

2. Explain how the Singleton pattern can be used with Node modules, specifically with classes.

   ```
   class PrivateSingleton {
       constructor() {
           this.message = 'I am an instance';
       }
   }

   class Singleton {
       constructor() {
           throw new Error('Use Singleton.getInstance()');
       }
   }

   static getInctance() {
       if(!Singleton.instance) {
           singletin.instance = new PrivateSingleton();
       }
       return Singletin.instance;
   }

   module.exports SingleTon.instance;

   ```

3. If you were tasked with building a middleware system like Express uses, what approach might you take to construct/operate it?

   - layers approach, building layers that communicate between each other.

## Vocabulary Terms

|          **Term**           |                                                                                                                             **Definition **                                                                                                                              |
| :-------------------------: | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
|      Router Middleware      |                                                                                                           function hand off the control to the next callback.                                                                                                            |
|   Dynamic Module Loading    | mechanism by which a computer program can, at run time, load a library (or other binary) into memory, retrieve the addresses of functions and variables contained in the library, execute those functions or access those variables, and unload the library from memory. |
|      Singleton Pattern      |                                          software design pattern that restricts the instantiation of a class to one "single" instance. This is useful when exactly one object is needed to coordinate actions across the system                                          |
| CRUD -> REST Method Matches |                                                                Create = PUT with a new URI POST to a base URI returning a newly created URI Read = GET Update = PUT with an existing URI Delete = DELETE                                                                 |
|        Mock Testing         |                                                             Mock testing is an approach to unit testing that lets you make assertions about how the code under test is interacting with other system modules                                                             |

##

- Securing Passwords
  `Bcrypt` hash password

  bcrypt was designed for password hashing hence it is a slow algorithm. This is good for password hashing as it reduces the number of passwords by second an attacker could hash when crafting a dictionary attack.

  - PROBLEMS WITH CRYPTOGRAPHIC HASH ALGORITHM

    - `Brute Force attack`

    - `Hash Collision attack`

    - `BCrypt, IT's SLOW AND STRONG AS HELL`

  This method of hashing passwords is solid enough for most web applications that stores users' passwords and other sensitive data.

2. Basic Auth
   \*is a method for an HTTP user agent (e.g. a web browser) to provide a user name and password when making a request. In basic HTTP authentication, a request contains a header field in the form of Authorization: Basic < credentials>, where credentials is the Base64 encoding of ID and password joined by a single colon :

   - Features

     HTTP Basic authentication (BA) implementation is the simplest technique for enforcing access controls to web resources because it does not require cookies, session identifiers, or login pages.

3. Authentication

   is the process of verifying that an individual, entity or website is whom it claims to be.

4. bcrypt docs
   npm package is one of the most used packages to work with passwords in JavaScript. This is security 101, but it's worth mentioning for new developers: you never store a password in plain text in the database or in any other place.
