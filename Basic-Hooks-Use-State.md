## Use State

### This hook allows us to control data in components by setting an initial state for every render and being able to target this value and use it for other components. This function uses events and event listeners to update the state.

## useState Example

```
import { useState } from 'react';
import ReactDOM from 'react-dom';

function ExampleComponent() {
  const [name, setName] = useState('Togara Hess');

  return
    <div>
      <p>Hello, {name}</p>
    </div>
}

ReactDOM.render(<ExampleComponent />, document.getElementById('root'));
```

## Screen View

## Hello Togara Hess
