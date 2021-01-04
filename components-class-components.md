## Class Components

### Class Components are used to apply logic to specified objects. These Components inherit given properties as hereditary characteristics. The latest Javascript syntax called ES6 is used in the application of Class Components. We refer to the method of delivering this logic to the screen as rendering.

## Example

```
index.js
```

```
import React from 'react';
import ReactDOM from 'react-dom';

class TextBook extends React.Component {
  render() {
    return <h1>Hello Humanoid!</h1>;
  }
}

ReactDOM.render(<TextBook />, document.getElementById('root'));
```

## Screen View

# Hello Humanoid !
