## Exp 9 – React Lab Exercise: React Fragments
## NAME: LIVYA DHARSHINI G
## REG NO: 2305001013
## Aim
To understand and implement React Fragments to group multiple JSX elements without creating
unnecessary HTML elements in the DOM.
## Objectives
1. Understand the concept of React Fragments.
2. Use Fragment shorthand syntax.
3. Use the explicit Fragment syntax.
4. Group multiple JSX elements without an extra DOM node.
5. Understand the difference between Fragments and div elements.
## Program
```
Step 1: Create a React Project

npm create vite@latest react-fragments
cd react-fragments
npm install
npm run dev

Select React as the framework and JavaScript as the variant.

Step 2: App.jsx – Using Fragment Shorthand

function Student() {
return (
<>
<h2>Student Details</h2>
<h3>Name: LIVYA DHARSHINI G</h3>
<p>Register Number: 2305001013</p>
      <p>Department: Computer Science and Engineering</p>
    </>
  );
}
function App() {
  return (
    <>
      <h1>College Information System</h1>
      <Student />
    </>
  );
}
export default App;

Step 3: Using Explicit Fragment Syntax

import { Fragment } from "react";
function Student() {
  return (
    <Fragment>
      <h2>Student Details</h2>
      <p>Name: LIVYA DHARSHINI G</p>
      <p>Department: CSE</p>
    </Fragment>
  );
}
function App() {
  return (
    <Fragment>
      <h1>College Information System</h1>
      <Student />
    </Fragment>
  );
}
export default App;
```
## Output
Fragment Shorthand Syntax

<img width="2112" height="745" alt="College Information System Student Details" src="https://github.com/user-attachments/assets/c7b512d9-3450-4452-86cc-bbeec6fefb4c" />


Explicit Fragment Syntax

<img width="2119" height="742" alt="Minimal College Information System Display" src="https://github.com/user-attachments/assets/57eb0640-2e07-45f0-85d1-53fc4210e166" />

## Result
Thus, React Fragments were successfully implemented using shorthand and explicit syntax to group
multiple JSX elements without creating unnecessary DOM elements.
