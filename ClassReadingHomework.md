# Reading Notes
A collection of my notes from codefellows

## Code 301 - Intermediate Software Development

### Read 01

Reading Questions

1. What is a “component”?
2. What are the characteristics of a component?
3. What are the advantages of using component-based architecture?
4. What is “props” short for?
5. How are props used in React?
6. What is the flow of props?

Reading Answer

i got this info from tutorialspoint.com/software_architecture_design/component_based_architecture.htm

1. A component is a modular, portable, replaceable, and reusable set of well-defined functionality that encapsulates its implementation and exporting it as a higher-level interface. 

2. Reusability, Replaceable, not context specific, extensible, encapsulated, independent

3. Ease of deployment, reduced cost, ease of development, resuable, modification of technical complexity, reliablity, Independent, System Maintenance and evolution.

4. Prop is short for properties

5. Props are used for passing data from one component to another

6. Uni-directional flow, it only flows from parent to child

### Read 02

Reading Questions 

1. Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?
2. What is the very first thing to happen in the lifecycle of React?
3. Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates
4. What does componentDidMount do?


5. What types of things can you pass in the props?
6. What is the big difference between props and state?
7. When do we re-render our application?
8. What are some examples of things that we could store in state?

Reading Answers

1. Render happens first

2. static getDerivedStateFromProps

3. constructor -> render -> componentDidMount -> React Updates -> componentWill Unmount

4. IF you need to load anything using a network request, it should go here, its a good place for subscriptions.

5. Any kind of data available in JS, number, boolean, object

6. Props get passed to the component (similar to funcitons parameters). State is managed within the component (similar to variables declared inside a function)

7. Re-rendering happens when react need to update the app with new data.

8. You can store any kind of JS value , including objects. 

### Read 03

Reading Questions

1. What does .map() return?
2. If I want to loop through an array and display each value in JSX, how do I do that in React?
3. Each list item needs a unique ____.
4. What is the purpose of a key?

5. What is the spread operator?
6. List 4 things that the spread operator can do.
7. Give an example of using the spread operator to combine two arrays.
8. Give an example of using the spread operator to add a new item to an array.
9. Give an example of using the spread operator to combine two objects into one.

Reading Answers

1. An entirely new array with transofrmed elements and the same amount of data

2. using the .map or for each loop

3. Key that uniquely identifies a list item among its siblings

4. Keys help react identify which items have been changed or added, or removed.

5. In Javascript spread syntax refers to the use of an ellipsis of three dots ... to expand an iterable object into the list of arguments.

6. Copy an Array, Concatenating arrays, using math funcitons, adding an item to a list

7. 
```
const myArray = [1, 2, 3];
const otherArray = [4, 5, 6];
const ourArray = [...myArray,...otherArray]
```

8. 
```
const myFood = ['pizza', 'steak', 'sushi'];
const moreFood = ['hotdog', 'hamburger', ...myFood];
```
9. 
```
const objectOne = {hello: "🤪"}
const objectTwo = {world: "🐻"}
const objectThree = {...objectOne, ...objectTwo, laugh: "😂"}
console.log(objectThree) // Object { hello: "🤪", world: "🐻", laugh: "😂" }
const objectFour = {...objectOne, ...objectTwo, laugh: () => {console.log("😂".repeat(5))}}
objectFour.laugh() // 😂😂😂😂😂
```
Source: https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab

### Read 04

Reading Questions

1. What is a ‘Controlled Component’?
2. Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.
3. How do we target what the user is entering if we have an event handler on an input field?
4. Why would we use a ternary operator?
5. Rewrite the following statement using a ternary statement:

Reading Answers:

1. Controlled Components are componentes that have access to the data the user entered in the form, while also handling the submit

2. Since the value attribute is set on our form element, the displayed value will always be this.state.value, making the React state the source of truth. Since handleChange runs on every keystroke to update the React state, the displayed value will update as the user types.

With a controlled component, the input’s value is always driven by the React state. While this means you have to type a bit more code, you can now pass the value to other UI elements too, or reset it from other event handlers. Source: https://reactjs.org/docs/forms.html

3. Event.target.value

4. We should use the ternary operator to shorten if statements, this allows us to specify which block of code to be executed if certain conditions are met.

5. 
```
(x===y) ? console.log(true) : console.log(false)
```