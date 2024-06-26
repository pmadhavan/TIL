### Today I Learned: React's key Prop and <Fragment> Tag
Today, I learned something new about the key prop in React, which I've been using for over six years. While I've always understood its importance in rendering lists in JSX for efficient updates, I discovered that the key prop does not appear in the actual DOM when viewed in the developer console. This was an interesting find, as it highlights that the key prop is used internally by React for its reconciliation process and isn't reflected in the DOM tree we can inspect in browser tools.

Additionally, I learned that this behavior is similar to React's <Fragment> tag, which also does not appear in the actual DOM. This similarity further illustrates how some React elements are used for organizational purposes in JSX but do not translate directly to visible DOM elements.

[Refer React official docs](https://react.dev/reference/react/Fragment#rendering-a-list-of-fragments)
