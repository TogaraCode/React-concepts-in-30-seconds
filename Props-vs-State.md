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
    return <h1>This textbook teaches {this.props.topic}!</h1>
  }
}

const exampleElement = <Textbook topic="React concepts in 30 seconds" />;

ReactDOM.render(exampleElement, document.getElementById('root'));
```

## Screen View

# This textbook teaches React Concepts in 30 Seconds

## State Example

```
index.js
```

```
import React from 'react';
import ReactDOM from 'react-dom';

class Textbook extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      topic: "React concepts in 30 seconds",
      volume: "1",
      Author: "Togara Hess",
      year: 2021
    };
  }
  render() {
    return (
      <div>
        <h1>This textbook teaches {this.state.topic}</h1>
        <p>
          Volume # {this.state.volume}
          written by {this.state.Author}
          published in {this.state.year}.
        </p>
      </div>
    );
  }
}

ReactDOM.render(<Car />, document.getElementById('root'));
```

## Screen View

# This textbook teaches React concepts in 30 seconds

## Volume #1 written by Togara Hess published in 2021
