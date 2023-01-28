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