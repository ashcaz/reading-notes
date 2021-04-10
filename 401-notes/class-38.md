# React 2

**LINKS**

- [React - Conditional Rendering](https://reactjs.org/docs/conditional-rendering.html)
- [React - Lists & Keys](https://reactjs.org/docs/lists-and-keys.html)
- [React - Forms](https://reactjs.org/docs/forms.html)
- [React - Lifting State](https://reactjs.org/docs/lifting-state-up.html)
- [React - Composition vs Inheritance](https://reactjs.org/docs/composition-vs-inheritance.html)
- [Thinking in React](https://reactjs.org/docs/thinking-in-react.html)

- [Hero Icons](https://www.youtube.com/watch?v=cVa1UiKPJN8)

- [React - Comprehensive Guide](https://tylermcginnis.com/reactjs-tutorial-a-comprehensive-guide-to-building-apps-with-react/)
- [Heroicons](https://heroicons.com/)

## Conditional Rendering

Conditional rendering in React works the same way conditions work in JavaScript. Use JavaScript operators like if or the conditional operator to create elements representing the current state, and let React update the UI to match them.

```JavaScript
function UserGreeting(props) {
  return <h1>Welcome back!</h1>;
}

function GuestGreeting(props) {
  return <h1>Please sign up.</h1>;
}
```

We’ll create a Greeting component that displays either of these components depending on whether a user is logged in:

```JavaScript
function Greeting(props) {
  const isLoggedIn = props.isLoggedIn;
  if (isLoggedIn) {
    return <UserGreeting />;
  }
  return <GuestGreeting />;
}

ReactDOM.render(
  // Try changing to isLoggedIn={true}:
  <Greeting isLoggedIn={false} />,
  document.getElementById('root')
);
```

## Lists and Keys

Given the code below, we use the `map()` function to take an array of `numbers` and double their values. We assign the new array returned by `map()` to the variable doubled and log it:

```JavaScript
const numbers = [1, 2, 3, 4, 5];
const doubled = numbers.map((number) => number * 2);
console.log(doubled);
```

This code logs [2, 4, 6, 8, 10] to the console.

[Back to Homepage](https://ashcaz.github.io/reading-notes)
