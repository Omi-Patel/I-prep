# React.js Concepts and Interview Questions

## Table of Contents

1. [Introduction to React.js](#introduction-to-reactjs)
2. [React.js Basics](#reactjs-basics)
   - [JSX](#jsx)
   - [Components](#components)
   - [State and Props](#state-and-props)
   - [Handling Events](#handling-events)
   - [Lists and Keys](#lists-and-keys)
   - [Forms](#forms)
3. [Advanced React.js](#advanced-reactjs)
   - [Hooks](#hooks)
   - [Context API](#context-api)
   - [Error Boundaries](#error-boundaries)
   - [Fragments](#fragments)
   - [React Router](#react-router)
   - [Higher-Order Components (HOCs)](#higher-order-components-hocs)
4. [Common Interview Questions](#common-interview-questions)
   1. What is React.js and why is it used?
   2. What is JSX in React?
   3. What is the difference between state and props?
   4. Explain the use of `useState` and `useEffect` hooks.
   5. What is the Virtual DOM?
   6. What are Higher-Order Components (HOCs)?
   7. What is the significance of keys in React?
   8. Explain how React handles forms.
   9. What is the Context API and how is it used?
   10. What are React Fragments?
   11. Explain the difference between controlled and uncontrolled components.
   12. What are error boundaries in React?
   13. How do you optimize performance in a React application?
   14. What is the role of `shouldComponentUpdate` in class components?
   15. What are React portals?

## Introduction to React.js

React.js is a popular JavaScript library for building user interfaces, particularly single-page applications. It allows developers to create reusable UI components and manage the view layer efficiently. React's component-based architecture makes code easy to maintain and debug.

---

## React.js Basics

### JSX

JSX stands for JavaScript XML. It allows you to write HTML elements inside JavaScript and place them in the DOM without `createElement()` or `appendChild()` methods. JSX is not mandatory in React but helps in building UI components more easily.

### Components

Components are the building blocks of a React application. They are JavaScript functions or classes that return HTML elements (via JSX) to be rendered on the screen. There are two types of components: Functional Components and Class Components.

### State and Props

- **State**: State is an object managed within a component. It determines how the component renders and behaves.
- **Props**: Props (short for properties) are read-only attributes passed from parent components to child components. Unlike state, props cannot be modified inside the child component.

### Handling Events

React events are similar to native DOM events but have some differences:

- Event names in React are written in camelCase, e.g., `onClick` instead of `onclick`.
- In JSX, you pass a function as the event handler, not a string.

### Lists and Keys

In React, when you create a list of elements, each element should have a unique "key" prop. Keys help React identify which items have changed, are added, or are removed, thus optimizing rendering performance.

### Forms

Handling forms in React involves controlled components where form data is handled by the component's state. The input field's `value` is controlled by the state, and updates are made through `onChange` events.

---

## Advanced React.js

### Hooks

Hooks are functions that allow you to use state and lifecycle methods in functional components. Common hooks include:

- `useState()`: Manages state in a functional component.
- `useEffect()`: Manages side effects in a functional component.
- `useContext()`: Consumes context values.

### Context API

Context API is a way to pass data through the component tree without having to pass props manually at every level. It's used for managing global state like theme, user authentication, etc.

### Error Boundaries

Error boundaries are React components that catch JavaScript errors anywhere in their child component tree and display a fallback UI instead of crashing the app.

### Fragments

Fragments allow you to return multiple elements from a component without adding extra nodes to the DOM. Use `<React.Fragment>` or shorthand `<> </>` to wrap elements.

### React Router

React Router is a library for handling navigation in a React application. It enables routing between different components and provides tools like `useHistory`, `useParams`, and `Link` for dynamic navigation.

### Higher-Order Components (HOCs)

A Higher-Order Component is a function that takes a component and returns a new component. HOCs are used for reusing component logic.

---

## Common Interview Questions

1. **What is React.js and why is it used?**
   React.js is a JavaScript library for building interactive user interfaces. It’s used for creating reusable UI components, managing the view layer in web applications, and handling the user interface efficiently.

2. **What is JSX in React?**
   JSX is a syntax extension for JavaScript that looks like HTML but is rendered as JavaScript objects. It allows you to write HTML-like code directly inside JavaScript, making it easier to create and visualize the UI.

3. **What is the difference between state and props?**

   - **State**: Mutable data that resides within a component.
   - **Props**: Immutable data passed from a parent component to a child component.

4. **Explain the use of `useState` and `useEffect` hooks.**

   - `useState`: Declares a state variable in functional components.
   - `useEffect`: Manages side effects such as data fetching, subscriptions, and manually changing the DOM.

5. **What is the Virtual DOM?**
   The Virtual DOM is a lightweight copy of the actual DOM. React uses the Virtual DOM to track changes in the component state and efficiently update the actual DOM only where necessary.

6. **What are Higher-Order Components (HOCs)?**
   HOCs are functions that take a component and return a new component with additional props or behavior. It allows for code reuse.

7. **What is the significance of keys in React?**
   Keys help React identify which items in a list have changed. It optimizes rendering performance by only re-rendering elements that have been updated.

8. **Explain how React handles forms.**
   React handles forms using controlled components where form data is handled via the component's state. Input values are updated via `onChange` events.

9. **What is the Context API and how is it used?**
   The Context API is used for passing data globally without passing props down manually at every level. It simplifies state management in cases where multiple components need access to the same data.

10. **What are React Fragments?**
    Fragments allow you to group a list of children without adding extra nodes to the DOM.

11. **Explain the difference between controlled and uncontrolled components.**

    - **Controlled Components**: Components where the form data is handled by the React state.
    - **Uncontrolled Components**: Components where the form data is handled by the DOM itself.

12. **What are error boundaries in React?**
    Error boundaries catch JavaScript errors in their child components and display a fallback UI instead of crashing the app.

13. **How do you optimize performance in a React application?**
    Use techniques like lazy loading, memoization (`React.memo`), and keeping components pure to optimize performance.

14. **What is the role of `shouldComponentUpdate` in class components?**
    `shouldComponentUpdate` allows you to optimize re-rendering by preventing unnecessary updates in class components.

15. **What are React portals?**
    React portals provide a way to render children into a DOM node that exists outside the hierarchy of the parent component.

---

This markdown file provides a comprehensive overview of React.js concepts and interview questions.
