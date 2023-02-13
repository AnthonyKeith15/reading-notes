#Answers to the questions in the reading

## Read 01

#### Compose a short poem describing how HTTP sends data between computers
```
I send a request
I recieve the web data
It comes in small bytes
```

#### Describe how HTML, CSS, and JS files are "parsed" in the browser.
```
-The browser begins with the HTML file, which looks for any references to outside files (external css or js).
-While the HTML is being parsed, it sends another request for the css files that have been found, and then any js. After it the browser parses the CSS and JS
-The browser generates a DOM and an in memory CCSOM structure, then compiles and executes JS
```

#### How can you find images to add to a website?
```
Go to google and use the image tab. Click on tools, then choose the *Creative Commons licenses* option. This is to reduce the likelihood of violating copyright.
```

#### How do you create a string vs a number in JavaScript?
```
Strings are enclosed in single or double quote marks
Numbers are not
```

#### What is a variable and why are they important in JavaScript?
```
Variables are containers that store values. They are important becuase you couldnt do anything personal or dynamic and fun.
```
#### What is an HTML attribute?
```
Attributes contain extra information about the element. However the attributes are not visible with the content.
```

#### Describe the anatomoy of an HTML element
```
1. The opening tag: the name of the element wrapped in opening and closing angle brackets.
2. The content: The content that we want displayed
3. The closing tag: like the opening tag, except with a forward slash where the element ends.
```

#### What is the difference between atricle and section tags?
```
"Article encloses a block of related content that makes sense on its own without the rest of the page (e.g., a single blog post)." [Source](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Document_and_website_structure)
Section is used for grouping together things that share one functionality. 
```

#### What Elements does a typical website include?
```
- Header
- Nav Bar
- Main Content
- Sidebar
- Footer
```

#### How does metadata influence Search Engine Optimization?
```
When using the Meta or title tag, it helps search engines pick out your website from the others as a better match.
```

#### How is the meta HTML tag used when specifying metadata?
```
The meta tag is used to provide keywords for search engines to determine relevance to that page for different terms.
```

#### What is the first step to designing a website?
```
The first step should be define what you want to accomplish with the website
```

#### What is the most important question to answer when designing a Website?
```
"What exactly do I want to accomplish?"
```

#### Why should you use an h1 element over a span element to display a top level heading?
```
Html sshould be representitive of the data that will be populated based on default styling. Cosmetics are the sole responsibilty of CSS
```

#### What are the benefits of using semantic tags in our HTML?
```
1. Search engines will consider its contesnts as important keywords to influence a pages ranking
2. Screen readers can use it as a signpost to help visually impaired users
3. Finding blocks of meaningful code is easier than searching through endless divs
4. Suggests to the devs the type of data that will be populated
5. Semantic naming mirrors proper custom element/component naming
```

#### Describe 2 things that *require* JavaScript in the browser?
```
1. Application Programming Interfaces (API)
2. Dynamic Behavior from a webpage
```

#### How can you add JavaScript to an HTML document?
```
By adding the script element to the HTML
```

## Read 02

#### Why is it important to use semantic elements in our HTML?
```
We rely on our previous experience to tell us what the function of an object is.
We also need to make sure we are using the correct elements, making sure the content has the correct label for screen readers and such.
```

#### How many levels of heading are there in HTML?
```
6
```

#### What are some uses for the *sub* and *sup* elements?
```
Sub = Subscript; This is used for smaller script such as chemical formulas
Sup = Superscript which is used for exponents or writing out dates with the "th" at the end
```

#### When using the *abbr* element, what attribute must be added to provide the full expansion of the term?
```
title
```

#### What are the ways we can apply CSS to our HTML?
```
1. External - Linking to an outside stylesheet
2. Internal - Writing the css at the top of our html file
3. Inline - writing our css in the same line as HTML
```

#### Why should we avoid using inline styles?
```
It is the opposite of a best practice, it is the least efficient way to implement. It is also more difficult to read and understand
```

#### Review the block of code below and answer the following questions  
1. What is representing the selector?
The h2 is the selector
2. Which components are the CSS declarations?
The CSS declaration is the key value pair of a CSS property and its value
3. Which components are considered properties?
The properties are the first item in the key value pair. This specifies what css property is changing
```
h2 {
  color: black;
  padding: 5px;
}
```

#### What data type is a sequence of text enclosed in single quote marks?
```
String
```

#### List 4 types of JS operators
```
1. Addition
2. Subtraction
3. Strict equality
4. Does-not-equal
```

#### Describe a real world problem you could solve with a function
```
I would make a function to cook me bacon in the morning so when I wake up it's hot and ready for me.
```

#### An if statement checks a __ and if it evaluates to ___, then the code block will execute.
```
Condition / True
```

#### What is the use of an Else If?
```
A way of providing more than one outcome for our if statement
```

#### List 3 different types of comparison operators
```
1. ===
2. > and <
3. <= and >=
```

#### What is the difference between the logical operator && and ||?
```
The && means *logical And* which means both expressions in it must be true or else it will return false
The || means *logical Or* which means either expression may be true and it will return true.
```

## Read 03

#### When should you use an unordered list in your HTML document?
```
The ul element is for grouping collections of items that don't have a need for numerical ordering. This could be a grocery list or a lineup at a concert.
```

#### How do you change the bullet style of unordered list items?
```
In CSS using the list-style-type property
```

#### When should you use an ordered list vs an unorder list in HTML documents?
```
Both OL and UL represent lists of items. Ol should be used when the order is meaningful, like a recipe or inststructions
UL are when the order does not matter
```

#### Describe two ways you can change the numbers on list items provided by an ordered list.
```
1. Using the type attribute
2. Using the reversed attribute
```

#### Describe the CSS properties of margin and padding as characters in a story. What is their role in a story titled: “The Box Model”?
```
In a story called the Box Model, The princess in the tower would be our content, the moat around the castle would be the border. The padding is the space between the castle and moat. Margin is the space outside of the moat to the next castle.
```

#### List and describe the four parts of an HTML elements box referred to by the box model.
```
Margin:
Border:
Padding:
Size:
```

#### What data types can you store inside of an Array?
```
Strings, numbers, objects and even other arrays
```

#### Is the people array a valid JavaScript array? If so, how can I access the values stored? If not, why?
```
Yes, you can access the values stored by people[0][0] if you need to access the array inside the array
```

#### List five shorthand operators for assignment in javascript and describe what they do.
```
1. x += f() | x = x + f() 
2. x -= f() | x = x - f()
3. x *= f() | x = x * f()
4. x /= f() | x = x / f()
5. x %= f() | x = x % f()
```
#### Read the code below and evaluate the last expression and explain what the result would be and why
```
10falsedog
Due to the order of operations in math, and JavaScript will just put all the phrases together as one string
```

#### Describe a real world example of when a conditional statemnet should be used in a JS program
```
If i am writing a program for a bank, I dont want them to be able to withdraw more money than they have. So i would need a conditions that checks if the withdraw amount is less than the total balance in the account.
```

#### Give an example when a loop is useful
```
A loop is usefull when you want to repeat things a certain amount of times
```

## Read 04

#### To create a basic link, we wrap text or other content inside what element?
```
Inside the a element and using the href attribute
```

#### The href attribute contains what information?
```
The target web address
```
#### What are some ways we can ensure links on our pages are accessible to all readers?
```
- Use clear link wording
- Dont repeat the url as part of the link text
- Dont say link in the link text
- Keep link as short as possible
```

#### What is meant by “normal flow”?
```
Normal flow is the way that webpage elements lay themselves out if you havent changed their layout
```

#### What are a few differences between block-level and inline elements?
```
The size of inline elements is just the size of their content
You cant set width or heigh on inline elements
```

#### ___ positioning is the default for every html element.
```
Static
```

#### Name a few advantages to using absolute positioning on an element
```
An absolute positioned element no longer exists in the flow of the document. Instead its got its own layer of the document.
Because of absolute positioning we can place the element exactly where we want it inside the containing element
```

#### What is a key difference between fixed positioning and absolute positioning?
```
Fixed will stay in one spot regardless of how far down you scroll on the page.
```

#### Describe the difference between a function declaration and a function invocation.
```
A declaration saves the name of the function and what happens when the function gets called.
The function invocation actually runs the line of code inside the function
```

#### What is the difference between a parameter and an argument?
```
A parameter is a value that gets passed into a function
An argument is the object that contains the values of the passed in parameter
```

#### Pick 2 benefits to pair programming and reflect on how these benefits could help you on your coding journey.
```
1. Engaged collaboration: Being able to collaborate with my peers who have different strengths will help me become a more well rounded student. This will also help me get over my fear of asking for help.
2. Social Skills: communication is a weak point for me. Being able to not only understand people better, but being able to be understood easier is a skill I know I will need later in life.
```

## Read 05

#### What is a real world use case for the alt attribute being used in a website?
```
Anyone using a screen reader will use the alt text to describe what is happening in the image since they cant see.
```

#### How can you improve accessibility of images in an HTML document?
```
By providing alt text and aria values. Also by wrapping the element in a relevant div will help users out alot.
```

#### Provide an example of when the figure element would be useful in an HTML document.
```
The figure tag contains self explanitory content, like diagrams, illustrations etc.
```

#### Describe the difference between a gif image and an svg image, pretend you are explaining to an elder in your community.
```
Gifs are similar to old school film, they only come in one resolution and it doesnt look as good as the digital counter part.
```

#### What image type would you use to display a screenshot on your website and why?
```
JPEG because it is the best choice and a fall back option. It has the most use cases. 
```

#### Describe the difference between foreground and background colors of an HTML element, pretend you are talking to someone with no technical knowledge.
```
Foreground are the things that appear closer to you, while the background is behind your main focus
```

#### Your friend asks you to give his colorless blog website a touch up. How would you use color to give his blog some character?
```
By using a limited color pallet and having a bright accent color. This will draw the users eyes to where we want to go.
```

#### What should you consider when choosing fonts for an HTML document?
```
Readablity, whether we need the serif or not. What the actual content on the page is.
```

#### What do font-size, font-weight, and font-style do to HTML text elements?
```
Font-size is how big the text itslef it.
Font-weight is how thick the lines are in the text
Font-style any extra saucy affects added to the text.
```

#### Describe two ways you could add spacing around the characters displayed in an h1 element.
```
margin/padding
line-height
```

## Read 6

#### How would you describe an object to a non-technical friend you grew up with?
```
An object is just a blueprint of code for another similar item we want to make.
```

#### What are some advantages to creating object literals?
```
Its useful for transfering a series of structured related data items
```

#### How do objects differ from arrays?
```
Arrays can be accessed by index number, objects can be accessed using dot notation
```

#### Give an example for when you would need to use bracket notation to access an object’s property instead of dot notation.
```
when the key pair label has a space in it
```

#### Evaluate the code below. What does the term this refer to and what is the advantage to using this?
```
this referes to the new object that is being created.
the advantage is we can access values of the object weve created using the dot notation
```

#### What is the dom?
```
The dom (document object model) is a rough tree of how elements on an html page are structed.
```

#### Briefly describe the relationship between the DOM and JavaScript.
```
You are able to use the DOM in order to save certain parts as a javascript variable and manipluate it
```

## Read 7

#### Explain why we need domain modeling.
```
It is neccesary to understand the specific problem that is being worked on so everyone involved can understand it.
```

#### Why should tables not be used for page layouts?
```
Layouts using tables make the website harder to navigate for screen readers.
```

#### List and describe 3 different semantic HTML elements used in an HTML table.
```
Thead - the head row of the table, has labels and defines the data
tbody - contains the data itself
tfoot - the last row of teh table, used for summarizing information
```

#### What is a constructor and what are some advantages to using it?
```
Its a way of creating multiple objects that all have similar data. The advantage is that if we needed to add a new property, it can be done easier in the constructor than having to go find every object literal
```

#### How does the term this differ when used in an object literal versus when used in a constructor?
```
this in a literal refers to the object itself
this in a constructor refers to the new instance of the object were creating
```

#### Explain prototypes and inheritance via an analogy from your previous work experience.
```
Prototypes are kindaa way of adding something on to a class as the last second and applying it to all the classes. In the military when theres a new standard thats the protype part. Inheritance is all the airman following the new standard.
```

## Read 8

#### Flexbox is designed for one-dimensional content. Explain what this means.
```
Flexbox is used to group like elements together in order to organize them on the page easier.
```

#### Explain the difference between the main axis and cross axis. 
```
The main axis is the axis of the direction our content is going
Cross axis is the perpendicular axis to that
```

#### How can using certain properties of flexbox negatively impact accessibility?
```
Using row reverse and column reverse only affect the page visually, for screen readers it will still be in a backwards order which makes things hard
```

#### What are some advantages of using flexbox over float?
```
You have way more control with flexbox of individual items over float.
```

#### How does this topic connect with your long term goals?
```
Any shorthand I can use will help save time when coding
```

## Read 9