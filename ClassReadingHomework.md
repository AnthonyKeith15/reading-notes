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