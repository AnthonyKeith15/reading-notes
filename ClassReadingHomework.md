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

Source: <https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab>

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

With a controlled component, the input’s value is always driven by the React state. While this means you have to type a bit more code, you can now pass the value to other UI elements too, or reset it from other event handlers. Source: <https://reactjs.org/docs/forms.html>

3. Event.target.value

4. We should use the ternary operator to shorten if statements, this allows us to specify which block of code to be executed if certain conditions are met.

5.

```
(x===y) ? console.log(true) : console.log(false)
```

### Read 05

1. A component should do one thing, it it ends up growing it should be broken down into smaller components.

2. Building a version without the use of state.

3. Think about the state that we need.

4. Is it passed in from a parent via props? If so, it probably isn’t state.
Does it remain unchanged over time? If so, it probably isn’t state.
Can you compute it based on any other state or props in your component? If so, it isn’t state.

5. Depending on what other information from other components it needs

CHANGE WEBSITE
6. A function that accepts functions as parameters and/or returns a function

7. returning m if m > n

8. The map method transforms and array by applying a function to all of its elements and building a new array from the returned values

### Read 06

1. Node.js is a JavaScript runetime built on Chromes v8 Js engine

2. Tis an open source Js engine that runs on google chrome as well as chrome adjacent browers.

3. Node.js is a program we can use to execute JS on our computers

4. NPM is a package manager that comes bundled with node

5. v19.6.1

6. 9.4.0

7. npm install -g jshint

8. Installing and running various build tools

9. 
```

Efficiency
Engaged Collaboration
Learning from fellow students
Social Skills
Job interview readiness
Work environment readiness

```
10. Social skills is the most important one. In the real world Im going to be working with other devs so knowing how to socialize is important.

11. One person handles all the actual coding, and nav of the files. The other person acts as a guide, in order to keep the big picture in mind as well as look up documentation. 

### Read 07

1. Roy Fielding helped write the first web servers, that sent documents across the internet. After that he did a ton of research explaining why the web works the way it does.

2. Theyre only hosted on our local server.

3. Its all about applying verbs to nouns. For instance when you go to a web page, the browser does an HTTP GET on the URL you typed in and back comes a webpage

4. They mostly just get stuff

5. Its when one system needs to add something to another system

6. If the system wants to replace something in another system.

7. Patch is kind of a partial update to the other systems

### Read 08

Representational State Transer


REST API are designed around resources, which are any kind of data, object and service that can be accessed by client

An identifier or a resource is a unique string of chars used to identify a specific resource. Example mysite.com/shopfield?9014 the stuff after the ? is the Identifier

GET POST PUT DELETE PATCH OPTIONS

URIs should be based on the things that they label EX: mysite.com/shop 

a chatty API makes multiple requests to do a single function. This is a bad thing because if you have slow internet it would take a long time to process these.

What status code does a successful GET request return?
200 code

What status code does an unsuccessful GET request return?
400 ish code depending on the specific problem 

What status code does a successful POST request return?
200 Code

What status code does a successful DELETE request return?
204 ?

### Read 09


1. Functional Programming is a programming paradigm - a style of building the structure and elements of computer programs. This treats computation as the evaluation of mathematical functions and avoids changing state and mutable data.

2. Its a pure function if it returns the same result if given the same arguments. It also does not cause any observable side effects

3. Were just accessing parameters passeed to the function, no external object

4. its state cannot change after its created.

5. When a pure function is passed with immutable data

6. A block of code that has a certain logical functionality. It essentially is just another js file

7. Require is on the global object. Its used to return the module.export from our module

8. require('./path-to-file')

9. module.export(exportedThing)

### Read 10

1. Its when a function is invoked (or called)

2. Since the stack is single function executions. Its done one at a time from top to bottom, meaning the stack is synchronous

3. Last in First out

Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.
4. 
```
function firstThing(){
  /* Stuff happens */
}

function secondThing(){
  firstThing();
  console.log('Im the second functon')
}

secondThing();

```
What causes a Stack Overflow?
5. When I get stuck on a bug it causes me to go to Stack Overflow lol.
It occurs when there is a recusive function without and exit point. The hosting environment has a max stack call before throwing an stack error


JavaScript error messages

6. When you try to use a variable that is not yet declared

7. It occurs when you have something that cannot be parsed in terms of syntax

8. Try to manipulate an object with some kind of length and give it an invalid length and youll get it.


9. Its when you try to access something undefined or not the correct data type.


10. Breakpoints are a conditional statement which will make your program stop at that point only if the condition is met.


11. The debugger keyword stops the execution of JavaScript, and calls (if available) the debugging function. This has the same function as setting a breakpoint in the debugger. If no debugging is available, the debugger statement has no effect. 

Source: https://www.w3schools.com/js/js_debugging.asp#:~:text=The%20debugger%20keyword%20stops%20the,debugger%20statement%20has%20no%20effect.

### READ 11

DIFFERENCES : SQL is a relational database
SQL databases are table based
SQL databases have a predefined schema
SQL databases use SQL
SQL databases are vertically scalable 

1.  SQL databases are good fit for the complex query intensive environment
2. Tax info
3. Non complex query
4. Cat info
5. NoSQL database fits better for the hierarchical data storage as it follows the key-value pair way of storing data
6. SQL databases are vertically scalable.

7. Structured Query Language
8. A relational database is a type of database that organizes data into one or more tables. which also has rows and columns to find things
9. a structured data model where data is organized into tables with predefined columns and data types.
10. a relational database is a collection of database objects, such as tables, indexes, and constraints, that define the structure of the database. 
11. database that stores and retrieves data without using a traditional relational database management system. Key value pairs
12. MongoDB is a document-oriented NoSQL database, meaning it stores data in JSON-like documents rather than tables with rows and columns. 
13. Mongo is more flexable because its not structred
14. Not as consistent and relaiable


### READ 12

100 = server got the request and is processing it
200 = SUCESS
300 = Resources got moved to somewhere else
400 = Errors that are the clients fault
500 = Errors that are the servers fault

202 = Your request has been accepted and still processing
308 = Lets you know that the resource moved to a new location.

If an updated didnt return data, it would a 204

If a resource doesnt exist its a 410

Forbidden is a 403. Not enough permissions.

1. We keep sensitive info in our env file so that it doesnt get added to our version control
2. Middleware is a function that sits between the client and the server in a web application.
3. This function is used to parse requests that are in JSON format
4. the /:id syntax specifies which parameter that can be used to capture a value from URL
5. PUT replaces an entire resource, PATCH updates part of it
6. By setting the default property in the field definition
7. Internal Server Error
8. 200 has successfully processed the request and is returning the resource. 201 means that the request is succesful and a new resource was created.

### READ 13

1. PUT
2. GET, PUT, DELETE, PATCH

3. CRUD is a set of operations mostly used by databases. REST uses CRUD operations to manage data in a uniform way.
4. Figure out what data I want. Find my end point. Choose the appropriate method that i need to use. Connect the front end to back and test that Im getting data. Test the api to make sure that I am getting the response Im expecting