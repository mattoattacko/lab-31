# lab-31
Created with CodeSandbox

### Links and Resources
* [Repo](https://github.com/mattoattacko/lab-31)
* [Assignment One](https://codesandbox.io/s/ov7v3nqryy)
* [Assignment Two](https://codesandbox.io/s/ykv771r7mx)

### Modules
## Assignment 1

#### `index.js`
##### Exported Values and Methods

###### `Main() -> <Provider>`
* The `app` component

#### `components/app.js`
##### Exported Values and Methods

###### `Class App -> <div>`
* Just the `div`

###### `mapStateToProps(state)`
* If state then state.someStuff

###### `mapDispatchToProps(dispatch, getState)`
* handleChange

###### `combineReducers()`
* Does what it sounds like

#### `store/reducers.js`
##### Exported Values and Methods

###### `export default()`
* If state, action have  CHANGE, it will return foo 
* If state, action are DEFAULT, it will return state

## Assignment 2

#### `index.js`
##### Exported Values and Methods

###### `Main() -> <Provider>`
* Our App component

#### `components/app.js`
##### Exported Values and Methods

###### `Class App -> <div>`
* We export into the app.js and render the div component

###### `mapStateToProps(state)`
* state.app

###### `mapDispatchToProps(dispatch, getState)`
* handleChange

#### `components/numbers.js`
##### Exported Values and Methods

###### `Class Numbers`
* The button?

###### `mapStateToProps(state)`
* state.numbers

###### `mapDispatchToProps(dispatch, getState)`
* If dispatch, getState, it will handleNumChange, then handleNumReset

#### `store/index.js`
##### Exported Values and Methods

#### `store/app-reducers.js`
##### Exported Values and Methods

###### `export default()`
<- state, action   -> if CHANGENAME, returns name || Math.random()    -> if DEFAULT, returns state

#### `store/app-actions.js`
##### Exported Values and Methods

###### `numberChanger()`
* CHANGENUM

###### `resetNumber()`
* RESET

#### Tests
* Tests
