## Lists and Keys

## Lists 

### If we were to over simply React we could describe it as consisting of many lists of items and data inside of lists of items and data like Russian dolls.Lists are commonly rendered inside components.We use the JSX .map() method to combine different types of data to update the DOM. For example, if we had a list of people's names and ages they would be two different types of data, names being words and ages being numbers. To arrange these names and numbers together we use the .map() function to combine these different types of data so that we can present them together in the DOM.

## List Example

```
index.js
```

```
import React from 'react';
import ReactDOM from 'react-dom';

function ExampleList(props) {
  const exampleList = props.exampleList;
  const listItems = exampleList.map((exampleList) =>
    <li>{exampleList}</li>
  );
  return (
    <div>
        <h1>This is an Example of a list</h1>
              <ol>{listItems}</ol>
    </div>
  );
}
const exampleList = ['Togara', '12', 'Aiyara', 'Lion', '500g'];
ReactDOM.render(
  <ExampleList exampleList={exampleList} />,
  document.getElementById('root')
);
```

## View on Screen

```
1 Togara
2 12
3 Aiyara
4 Lion
5 500g
```

## Keys

###  A Key is used to target and label an item in a list by giving it an ID. We also use keys to monitor changes in specific items in lists. An easy way to remember how we use Keys in React is the same way we use keys to unlock doors. Using this analagy we can imagine that a key only works for a specific lock.

## Key Example

```
index.js
```

```
import React from 'react';
import ReactDOM from 'react-dom';

function ExampleItem(props) {
  const item = props.item;
  return (
    <li> {item} </li>
  );
}
function ExampleList(props) {
  const exampleList = props.exampleList;
  const exampleItems = exampleList.map((strList) =>
    <ExampleItem key={exampleList.toString()} item={strList} />
  );
  return (
    <div>
        <h1>This is an Example of Keys</h1>
            <ol>{exampleItems}</ol>
    </div>
  );
}
const exampleList = ['Togara', 'Mandela', '12', 'Orange', '500g'];
ReactDOM.render(
  <ExampleList exampleList={exampleList}/>,
  document.getElementById('root')
);

```

## View on Screen

# This is an Example of Keys

### 1. Togara

### 2. Mandela

### 3. 12

### 4. Orange

### 5. 500g
