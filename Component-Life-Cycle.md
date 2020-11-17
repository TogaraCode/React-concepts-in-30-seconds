## Component Life Cycle

### Every component has a life cycle that is divided into three phases.

### The first is the creation phase, called Mounting. 

### The second phase is called Updating.

### The third and last is the deletion phase called Unmounting.

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
