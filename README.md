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
-> App Component

#### `components/app.js`
##### Exported Values and Methods

###### `Class App -> <div>`
-> div

###### `mapStateToProps(state)`
<- state   -> stuff: state.someStuff

###### `mapDispatchToProps(dispatch, getState)`
<- dispatch, getState    -> handleChange

#### `store/actions.js`
##### Exported Values and Methods

###### `changer(payload)`
<- payload    -> type: 'CHANGE'   -> payload

#### `store/index.js`
##### Exported Values and Methods

###### `combineReducers()`
-> someStuff

#### `store/reducers.js`
##### Exported Values and Methods

###### `export default()`
<- state, action    -> if CHANGE, returns foo    -> if DEFAULT, returns state

## Assignment 2

#### `index.js`
##### Exported Values and Methods

###### `Main() -> <Provider>`
-> App Component

#### `components/app.js`
##### Exported Values and Methods

###### `Class App -> <div>`
-> div    -> Numbers Component

###### `mapStateToProps(state)`
<- state      -> app: state.app

###### `mapDispatchToProps(dispatch, getState)`
<- dispatch, getState     -> handleChange

#### `components/numbers.js`
##### Exported Values and Methods

###### `Class Numbers`
-> div     -> button

###### `mapStateToProps(state)`
<- state   -> numbers: state.numbers

###### `mapDispatchToProps(dispatch, getState)`
<- dispatch, getState  -> handleNumChange    -> handleNumReset

#### `store/index.js`
##### Exported Values and Methods

###### `combineReducers()`
-> app     -> numbers

#### `store/app-reducers.js`
##### Exported Values and Methods

###### `export default()`
<- state, action   -> if CHANGENAME, returns name || Math.random()    -> if DEFAULT, returns state

#### `store/app-actions.js`
##### Exported Values and Methods

###### `nameChanger(payload)`
<- payload

-> type: CHANGENAME

-> payload

#### `store/numbers-reducers.js`
##### Exported Values and Methods

###### `export default()`
<- state, action

-> if CHANGENAME, returns name || Math.random()

-> if RESET, returns initialState

-> if DEFAULT, returns state

#### `store/numbers-actions.js`
##### Exported Values and Methods

###### `numberChanger()`
-> type: CHANGENUM

###### `resetNumber()`
-> type: RESET

#### Tests
* 
