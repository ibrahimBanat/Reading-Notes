## Component Composition

1 - Can a parent component access the state of a child component?
In React we can access the child's state using Refs. we will assign a Refs for the child component in the parent component. then using Refs we can access the child's state.

2 - What can be passed along in a prop variable?
Everything such as property or a method.

3 - How can a child component “know” the state of another component?
component props: What we pass from the parent component to the child component to can access them.

component state: Its a object specific to the one components.

application state: Represent all the state of the application.

## Vocabulary Terms

Word Definition
component props: Props are arguments passed into React components. Props are passed to components via HTML attributes.
component state: an object that determines how that component renders & behaves. In other words, “state” is what allows you to create components that are dynamic and interactive.
application state represents the totality of everything necessary to keep your application running

## React Basic

- Mounting

Since class-based components are classes, hence the name, the first method that runs is the constructor method. Typically, the constructor is where you would initialize component state.

Next, the component runs the getDerivedStateFromProps. I’m going to skip this method since it has limited use.

Now we come to the render method which returns your JSX. Now React “mounts” onto the DOM.

Lastly, the componentDidMount method runs. Here is where you would do any asynchronous calls to databases or directly manipulate the DOM if you need. Just like that, our component is born.

- Updating

This phase is triggered every time state or props change. Like in mounting, getDerivedStateFromProps is called (but no constructor this time!).

Next shouldComponentUpdate runs. Here you can compare old props/state with the new set of props/state. You can determine if your component should re-render or not by returning true or false. This can make your web app more efficient by cutting down on extra re-renders. If shouldComponentUpdate returns false, this update cycle ends.

If not, React re-renders and getSnapshotBeforeUpdate runs afterwards. This method has limited use as well. React then runs componentDidUpdate. Like componentDidMount you can use it to make any async calls or manipulate the DOM.

- Unmounting

Our component lived a good life, but all good things must come to an end. The unmounting phase is that last stage of the component lifecycle. When you remove a component from the DOM, React runs componentWillUnmount right before it gets removed.

- Props.children
  props.children is a special prop, automatically passed to every component, that can be used to render the content included between the opening and closing tags when invoking a component

- Composition vs Inheritance
  Inheritance

Those familiar with Object Oriented Programming are well aware of Inheritance and use it on a regular basis. When a child class derives properties from it’s parent class, we call it inheritance. There are variety of use-cases where inheritance can be useful.

- Composition

Composition is also a familiar concept in Object Oriented Programming. Instead of inheriting properties from a base class, it describes a class that can reference one or more objects of another class as instances.
