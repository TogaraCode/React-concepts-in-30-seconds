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

#

```
index.html
```

```
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8" />
    <meta name="viewport"
      content="width=device-width, initial-scale=1" />
    <title>React App</title>
  </head>
  <body>

    <div id="root"></div>

  </body>
</html>
```

## Screen View

# Hello Humanoid !
