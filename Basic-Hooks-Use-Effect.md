## Use Effect

### This Hook is used to target parts of an object that we want to change on every render(). The useEffect function interacts directly with the DOM and has access to every phase in the component's lifecycle. We use this hook to handle the change in the state of the component.

## useEffect Example

```
import React, { useState, useEffect } from 'react';
import ReactDOM from 'react-dom';

const Example = () => {
  const [greeting, setGreeting] = useState('Hello Huminoid');

  useEffect(() => {
    console.log('activate first greeting');

    setTimeout(() => {
      setGreeting("Welcome to the future");
    }, 420)
  }[]);

  return <h1>{greeting}</h1>
};

ReactDOM.render(<Example />, document.getElementById('root'));

```

## Screen View

# Hello Humanoid

```
after 420 seconds the screen will show
```

# Welcome to the future
