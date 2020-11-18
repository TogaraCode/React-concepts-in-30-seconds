## Component Life Cycle

### Every component has a life cycle that is divided into three phases.

### 1.The first is the creation phase, called Mounting. 

### 2.The second phase is called Updating.

### 3.The third and last is the deletion phase called Unmounting.

### A method is a function that has its own properties/characteristics.

### React uses methods in the lifecycle called Lifecycle Methods. 

## Phase 1 - Mounting 

### Mounting is when we insert a component into HTML and XML, also referred to as the DOM.

### React calls four methods in consecutive order when mounting components.It is important to note that although all four Methods are available to us, only one of them called the render() method is mandatory.

### 1.constructor()

### 2.getDerivedStateFromProps()

### 3.render()

### 4.componentDidMount() 

## 1. constructor()

### The constructor() method is what we use to create the Class and introduce the initial object to the DOM.

## 2. getDerivedStateFromProps() 

### This method is always called before the render() method. It is not recommended because it is very expensive. It checks to see if the state of any props have changed in order to decide what its output will be accordingly. We avoid using this method because it is put to work on every render() to check for a change in state and this is unnecessary when the props have not changed.

## 3. render()

### This is the only mandatory method that needs to be called in a components life cycle.What the render() method does is it takes the data from props and state and returns it into the Dom.

## 4.componentDidMount()

### This method comes after the first render() and allows us to apply any changes to the initial state. Javascript logic is used to change the state before replacing the result back  into the Dom.

## Phase 2. Updating

### This phase comes into play when changes or updates are made to the initial state of the component.

### React calls five methods in consecutive order when updating components. It is important to note that although all four Methods are available to us, only one of them called the render() method is mandatory.

### 2.1.static getDerivedStateFromProps()

### 2.2.shouldComponentUpdate()

### 2.3.render()

### 2.4.getSnapshotBeforeUpdate()

### 2.5.componentDidUpdate()

## 2.1. static getDerivedStateFromProps()

### This method is used before every render() including the initial mounting. What this method does is it looks for any change in data resulting in a state being updated and it returns the updated state. 

## 2.2. shouldComponentUpdate()

### This method is used to avoid unnecessary rendering() when props have not changed. If there are no updates in data then this method will recognize this and stop further rendering(). In other words, if the state of all the properties stay the same then this method will notice this by using Javascript true or false statements and if it is true that all the data stays the same then this method will disallow any further rendering.

## 2.3 render()

### This is the only mandatory method that needs to be called in a components life cycle.What the render() method does is it takes the data from props and state and returns it into the Dom.

## 2.4 getSnapshotBeforeUpdate()

### What this method does is it looks at the previous render() and checks if any changes or updates were made in the DOM.If any changes were made in the DOM then this method captures those changes and stores it as a value called snapshot, to be used in the next step in updating the component.

## 2.5. componentDidUpdate()

### This is the final step in updating a component. What this method does is it takes all the updates and changes made and replaces the old values with the new changes in the DOM.

## 3.1 componentWillUnmount()

### This phase is used to delete/remove the object from the Dom.
