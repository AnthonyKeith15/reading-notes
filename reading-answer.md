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