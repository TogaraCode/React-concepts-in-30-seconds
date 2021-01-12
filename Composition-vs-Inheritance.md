## Compostion vs Inheritance

## Composition

### Composition is a pattern we use to target and manipulate one or more Class Components.  We can build Components inside Components and add specific properties to these objects inside of objects as we go along. This pattern can continue indefinitely. This is used in object-oriented programming (OOP). Composition is the cleanest and most preferred practice in writing code.

## Composition Example

```
import React from 'react';
import ReactDOM from 'react-dom';

class Playlist extends React.Component {

  render() {
    return (
      <div className="playlist">
        <Artist />
        <Album />
        <Song />
      </div>
    );
  }

}

ReactDOM.render(<Playlist />, document.getElementById('root'));

```

## Inheritance

### This pattern makes use of Child Components that take on the properties of Parent Components.This style of writing code is not recommended because React has a Component-based structure and Composition is more suitable in this type of environment.  
