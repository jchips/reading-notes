# Reading Notes 26: Component Based UI

This topic is important because it talks about the basics of React which is what we will use for frontend development.

Note: There are no classes 20-25.

## [React Quick Start](https://react.dev/learn)

What are the building blocks of a React app?

- The building blocks of a React app are components. A component is a piece of the UI that has its own logic and appearance. React components are JavaScript functions that return markup.

What is the difference between an HTML element and a React component?

- React elements start with a capital letter and HTML elements are all lowercase.

What is JSX and why do we use it?

- JSX is a markup syntax similar to HTML but stricter. It allows "escaping into JavaScript" while coding in React so one can put markup into JavaScript.

Describe the process of embedding JavaScript expressions in JSX.

- Below is an example that I modified from <https://react.dev/learn>:

```javascript
function AboutPage() {
  return (
    <>
      <h1>About</h1>
      <p>Hello there.<br />How do you do {user.name}?</p>
    </>
  );
}
```

Does React or JSX have any special features for iteration or conditional logic?

- For conditional logic in React, one can use the tenary operator or the `&&` symbol in JSX.
- For iteration, one can use the array map function with JSX. When using the array map function in React, leave out the curly brackets. Also, for each item in the list, there must be a `key` attribute.

How does React know to respond to a user’s inputs?

- By devs adding event handler functions in the components. Then the dev can pass down the handler function in the JSX.

What word indicates that a React component manages data with a Hook?

- The word `use`. Functions starting with `use` are called Hooks in React.

How can two react components share data?

- By moving the state storing the data into the closest parent component for both components.

## [Render and Commit](https://react.dev/learn/render-and-commit)

What are the three steps of refreshing a React UI?

1. Trigger a render
2. React performs the render
3. React commits changes to the DOM

How do you trigger updates to a component after the initial render?

- By updating the state.

Does React recreate DOM nodes on every rerender?

- No, React only changes the DOM nodes if there’s a difference between renders.

After React has updated the DOM, what still needs to happen before the user sees the change?

_ The browser will repaint the screen. This is called "browser rendering".

## Additional Questions

1. Note the naming conventions in the Airbnb React/JSX Style Guide. What pattern(s) do you see?

- .jsx extension for React components.
- PascalCase for filenames and React components.
- camelCase for instances of React components.
- Prop names shouldn't be the same as DOM prop names (like `className` or `style`).

2. Looking ahead at this module’s course schedule, What do you look forward to learning?

- Learning SASS because I already use SCSS with some projects but I don't use all its features yet, learning about Vite, and using the Reducer hook because I've used it before but I want more practice and a better understanding of it.

3. What are your learning goals after reading and reviewing the class README?

- My learning goal is to learn about Vite and understand SASS better.

## Things I want to know more about
