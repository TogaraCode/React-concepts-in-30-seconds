## Components

### We divide websites into objects that fit together like pieces of a puzzle. This is done so that we can target different items on the website especially when we would like different elements of the website to serve independent specific functions. Components are also very useful because of their reusable nature allowing us to duplicate elements on the website.

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
