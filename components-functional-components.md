## Functional Components

### A Functional Component is a set of rules that we can allocate to specific objects on a website. Its purpose is to return an element onto the screen.We can designate specific characteristics, called props(properties) to these particular sections. JSX is used to present an argument to manipulate the function of these particular objects and present the desired outcome onto the screen.

## Example

```
index.js
```

```
import React from 'react';
import ReactDOM from 'react-dom';

function TextBook() {
  return <h1>Hello Humanoid!</h1>;
}

ReactDOM.render(<TextBook />, document.getElementById('root'));
```

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
