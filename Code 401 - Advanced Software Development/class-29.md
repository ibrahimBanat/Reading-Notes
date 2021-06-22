# Routing

## 1 - Do child components have direct access to props/state from the parent?

**Actually not direct access but by pass its state as a props to the child.**

## 2 - When a component “wraps” another component, how does the child component’s output get rendered? 

      <Main>
        <Content/>
      </Main>

**By add the component as a children props**

## 3 - Can a component, such as `<Content />`, which is a child also be used as a standalone component elsewhere in the application?

**Yes,It can be reused**

## 4 - What trick can a parent use to share all props with it’s children


---


## Important Terms


Word | Definition 
------------ | -------------
props.children |  allows to pass a component or markup as a props to children

composition | is a natural pattern of the component model. It's how we build components from other components, of varying complexity and specialization through props. Depending on how generalized these


---

## React Router

**The component is the main building block of React Router. Anywhere that you want to only render content based on the location’s pathname, you should use a element.**

- Choosing our router
- Creating our routes
- Navigating between routes using links

---

## Hooks


**useHistory**

*The useHistory hook gives you access to the history instance that you may use to navigate.*

**useLocation**

*The useLocation hook returns the location object that represents the current URL. You can think about it like a useState that returns a new location whenever the URL changes*.

**useParams**

*useParams returns an object of key/value pairs of URL parameters. Use it to access match.params of the current route.*

---

# THE END 