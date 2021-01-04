## Conditional Rendering

### Conditional Rendering is used to manage the change in specified components displayed on the screen. We can also target aspects of a component and manipulate a change within the object while retaining the remaining initial components' composition. Stateful Components are used in this case, meaning the properties of the element will be updated, depending on whether the specified data in the element has changed or not. The Javascript expressions, "If true or false, statements", are used as a binary deciding factor resulting in the rendered output. 

## Example

```
import React from 'react';
import ReactDOM from 'react-dom';

function UserEnglish(props) {
  return <h1>Good Morning!</h1>;
}

function UserGerman(props) {
  return <h1>guten Morgen!</h1>;
}

function Language(props) {
  const isUserEnglish = props.isUserEnglish;
  if (userEnglish) {
    return <UserEnglish />;
  }
  return <userGerman />;
}

ReactDOM.render(
  <Language isUserEnglish={false} />,
  document.getElementById('root')
);

```

## View on Screen

# guten Morgen!
