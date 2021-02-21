# Object Literals and the DOM

What is an object in JavaSCript?

*Object*:

  Objects are representations of real world things that are made using variables and functions that are grouped together.

  Variables and functions used within objects operate the same way but are called by different names. In an object, a variable is called a property.

*Property:*

  Properties give information about the object like what the name of a park is. The park would be the object and the name *Pennyhill* would be the name or property of the park.

*Functions:*

  Within an object, functions are known as "methods". Methods are used to do tasks within the object. For instance, if you wanted to know how many more trees need to be planted in a park to get a total number of trees, you'd look at the total number of trees needed and then subtract the current number of trees planted.

Now that we have a bit of information about objects, let's look at how to create one. There are many ways to do this. Below is just one way to do this.

```var park = {```

  ```name: 'Pennyhill',```

  ```trees-needed: 60,```

  ```trees-planted: 20,```

  ```checkTotalneeded: function() {```

  ```return this.treesPlanted - this.treesNeeded;```

  ```}```

```};```

Accessing the object's properties or method is done using what is called "dot notation". This means that the name of the object, followed by a period (. "dot") and then the name of the method or property you are trying to access.

For example:

```var parkName = park.Pennyhill```

```var totalNeeded = park.checkTotalneeded();```

This can also be done using square brackets [].

```var parkName = park['Pennyhill']```

```var totalNeeded = park['checkTotalneeded']();```

Up next...

## Dom, Dom Dommmmmmm

**DOM**: Document Object Model, dictates how the browser  creates a model of an HTML page and how JavaScript accesses and updates the webpage while in the borwser window.

  DOM models are stored in the browsers memory

  DOMs have four different nodes:

    Document Node

    Element Node

    Attribute Node

    Text Node

Each node is an object with properties and methods.
     
## Summary
- The browser represents the page using a DOM tree.
DOM trees have four types of nodes: document nodes,
element nodes, attribute nodes, and text nodes.
- You can select element nodes by their id or cl ass
attributes, by tag name, or using CSS selector syntax.
Whenever a DOM query can return more than one
node, it will always return a Nadel i st.
- From an element node, you can access and update its
content using properties such as textContent and
i nnerHTML or using DOM manipulation techniques.
- An element node can contain multiple text nodes and
child elements that are siblings of each other.
- In older browsers, implementation of the DOM is
inconsistent (and is a popular reason for using jQuery).
Browsers offer tools for viewing the DOM tree . 