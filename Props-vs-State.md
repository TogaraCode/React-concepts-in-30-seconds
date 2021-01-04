## Props vs State

### Props as previously mentioned is an abbreviation of the word properties. We use these as a set of rules we wish to apply to specified objects/components as initial static arguments. 

### State is used as an argument when we foresee an intended change in data. We use State as a tool to control the change in the component and manage the rendered output. 

## Props Example

```
index.js
```

```
import React from 'react';
import ReactDOM from 'react-dom';

class Textbook extends React.Component {
  render() {
    return <h1>This Computer Science Textbook teaches {this.props.topic}!</h1>
  }
}

const myelement = <Textbook topic="React concepts" />;

ReactDOM.render(myelement, document.getElementById('root'));
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

# This Computer Science textbook teaches React Concepts
