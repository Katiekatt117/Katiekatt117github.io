# *Websites for 201 Class 1*

- https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/How_the_Web_works


- https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/What_will_your_website_look_like


- https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/JavaScript_basics


- https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/The_head_metadata_in_HTML


- https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Getting_started


- https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Selectors


- https://developer.mozilla.org/en-US/docs/Web/HTTP


https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML


https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Getting_started


https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Document_and_website_structure




# **My Poem On HTTP**

Hypertext Transfer Protocol is an application protocol that defines a language for clients and servers to speak to each other

Without it, how could computers work together?

The browser sends an HTTP request message to the server, asking it to send a copy of the website to the client 

It is very reliant!

It helps you get to the places you want to go,

And understand the things you want to know!



# **Order in which component files are parsed**


When browsers send requests to servers for HTML files, those HTML files often contain **< link>** elements referencing external CSS stylesheets and **< script>** elements referencing external JavaScript scripts. It's important to know the order in which those files are parsed by the browser as the browser loads the page:

- The browser parses the HTML file first, and that leads to the browser recognizing any **< link>**-element references to external CSS stylesheets and any **< script>**-element references to scripts.

- As the browser parses the HTML, it sends requests back to the server for any CSS files it has found from **< link>** elements, and any JavaScript files it has found from **< script>** elements, and from those, then parses the CSS and JavaScript.

- The browser generates an in-memory DOM tree from the parsed HTML, generates an in-memory CSSOM structure from the parsed CSS, and compiles and executes the parsed JavaScript.

- As the browser builds the DOM tree and applies the styles from the CSSOM tree and executes the JavaScript, a visual representation of the page is painted to the screen, and the user sees the page content and can begin to interact with it.


# **How To Add Images**


To choose an image, go to **Google Images** and search for something suitable.

1.) When you find the image you want, click on the image to get an enlarged view of it.

2.) Right-click the image (Ctrl + click on a Mac), choose *Save Image As…*, and choose a safe place to save your image. Alternatively, copy the image's web address from your browser's address bar for later use.

## **Note**

 - that most images on the web, including in Google Images, are copyrighted. To reduce your likelihood of violating copyright, you can use Google's license filter. Click on the *Tools* button, then on the resulting *Usage rights* option that appears below. You should choose the option *Creative Commons licenses*.



# **Creating a string**


1.) To start with, enter the following lines:

- const string = **"The revolution will not be televised."**;

- console.log(string);

*Just like we did with numbers, we are declaring a variable, initializing it with a string value, and then returning the value. The only difference here is that when writing a string, you need to surround the value with quotes.*

2.) If you don't do this, or miss one of the quotes, you'll get an error. Try entering the following lines:

- const badString1 = This is a test;

- const badString2 = 'This is a test;

- const badString3 = This is a test';

These lines don't work because any text without quotes around it is assumed to be a variable name, property name, a reserved word, or similar. If the browser can't find it, then an error is raised (e.g. "missing; before statement"). If the browser can see where a string starts, but can't find the end of the string, as indicated by the 2nd quote, it complains with an error (with "unterminated string literal"). If your program is raising such errors, then go back and check all your strings to make sure you have no missing quote marks.

3.) The following will work if you previously defined the variable **string** — try it now:

- const badString = string;

- console.log(badString);

**badString** is now set to have the same value as **string**.


# **Numbers vs. strings**


So what happens when we try to combine a string and a number? Let's try it in our console:

- const name = **"Front "**;

- const number = **242**;

- console.**log**(`${name}${number}`); // "Front 242"


You might expect this to return an error, but it works just fine. Trying to represent a string as a number doesn't really make sense, but representing a number as a string does, so the browser converts the number to a string and concatenates the two strings.

If you have a numeric variable that you want to convert to a string but not change otherwise, or a string variable that you want to convert to a number but not change otherwise, you can use the following two constructs:

The **Number()** function converts anything passed to it into a number, if it can. Try the following:

- const myString = **"123"**;

- const myNum = **Number**(myString);

- console.**log**(typeof myNum);


Conversely, every number has a method called **toString()** that converts it to the equivalent string. Try this:

- const myNum2 = **123**;

- const myString2 = myNum2.**toString()**;

- console.**log**(typeof myString2);


These constructs can be really useful in some situations. For example, if a user enters a number into a form's text field, it's a string. However, if you want to add this number to something, you'll need it to be a number, so you could pass it through **Number()** to handle this.

# **What is a variable and why is it important in JavaScript?**

In JavaScript, variables are used to hold a value. It can hold any value, from primitives to objects. The = sign in JavaScript isn't the same as the = sign in Math. In JavaScript, = means assignment.

## **Why It's Important**

In JavaScript, variables are used to hold a value. It can hold any value, from primitives to objects. The = sign in JavaScript isn't the same as the = sign in Math. In JavaScript, = means assignment.

# **Why is it important to declare a variable?**

The main purpose of variable declaration is to store the required data in the memory location in the form of variables so that we can use them in our program to perform any operation or task. By declaring a variable, we can use that variable in our program by using the variable name and its respective data type.

# **What is an example of a variable in JavaScript?**

In JavaScript, we use either var or let keyword to declare variables. For example, var x; let y; Here, x and y are variables.

# **Why is it important to declare a variable in Java?**

You have to tell Java the type of the variable because Java needs to know how many bits to use and how to represent the value.


# **What is an HTML attribute?**

HTML attributes are special words used inside the opening tag to control the element's behaviour. HTML attributes are a modifier of a HTML element type. An attribute either modifies the default functionality of an element type or provides functionality to certain element types unable to function correctly without them.

# **What is HTML?**

There are 6 levels of heading in HTML

At its heart, HTML is a language made up of elements, which can be applied to pieces of text to give them different meaning in a document (Is it a paragraph? Is it a bulleted list? Is it part of a table?), structure a document into logical sections (Does it have a header? Three columns of content? A navigation menu?), and embed content such as images and videos into a page.

### **HTML**

 (HyperText Markup Language) is a markup language that tells web browsers how to structure the web pages you visit. It can be as complicated or as simple as the web developer wants it to be. HTML consists of a series of elements, which you use to enclose, wrap, or mark up different parts of content to make it appear or act in a certain way. The enclosing tags can make content into a hyperlink to connect to another page, italicize words, and so on. For example, consider the following line of text:

### **HTML** - Hypertext Markup Language, a standardized system for tagging text files to achieve font, color, graphic, and hyperlink effects on World Wide Web pages.
*"an HTML file"*

# **Anatomy of an HTML element**

## *The anatomy of our element is:*

- **The opening tag:**
This consists of the name of the element (in this example, p for paragraph), wrapped in opening and closing angle brackets. This opening tag marks where the element begins or starts to take effect. In this example, it precedes the start of the paragraph text.

- **The content:**
This is the content of the element. In this example, it is the paragraph text.

- **The closing tag:** This is the same as the opening tag, except that it includes a forward slash before the element name. This marks where the element ends. Failing to include a closing tag is a common beginner error that can produce peculiar results.

The element is the opening tag, followed by content, followed by the closing tag.

# **What is the difference between article and section element tags in HTML?**

***The article tag is used for wrapping an autonomous content on a page.*** A content is autonomous if it can be removed from the page and put on some another page. The section tag is similar to the div tag, but it is more meaningful since it wraps logical groups of related content (e.g. a chapter of an article).


# **Elements That a Typical Website Would Have**

1.) Curated navigation menu

2.) Clear call to action

3.) Scannable typography

4.) Purposeful Visuals

5.) Strategic color scheme

6.) Responsive web design

7.) Interactive elements

8.) Authentic about page

9.) Accessible contact page

10.) SEO elements

11.) Website analytics

Webpages can and will look pretty different from one another, but they all tend to share similar standard components, unless the page is displaying a fullscreen video or game, is part of some kind of art project, or is just badly structured:

- **header:**
Usually a big strip across the top with a big heading, logo, and perhaps a tagline. This usually stays the same from one webpage to another.

- **navigation bar:**
Links to the site's main sections; usually represented by menu buttons, links, or tabs. Like the header, this content usually remains consistent from one webpage to another — having inconsistent navigation on your website will just lead to confused, frustrated users. Many web designers consider the navigation bar to be part of the header rather than an individual component, but that's not a requirement; in fact, some also argue that having the two separate is better for accessibility, as screen readers can read the two features better if they are separate.

- **main content:**
A big area in the center that contains most of the unique content of a given webpage, for example, the video you want to watch, or the main story you're reading, or the map you want to view, or the news headlines, etc. This is the one part of the website that definitely will vary from page to page!

- **sidebar:**
Some peripheral info, links, quotes, ads, etc. Usually, this is contextual to what is contained in the main content (for example on a news article page, the sidebar might contain the author's bio, or links to related articles) but there are also cases where you'll find some recurring elements like a secondary navigation system.

- **footer:**
A strip across the bottom of the page that generally contains fine print, copyright notices, or contact info. It's a place to put common information (like the header) but usually, that information is not critical or secondary to the website itself. The footer is also sometimes used for SEO purposes, by providing links for quick access to popular content.

To implement such semantic mark up, HTML provides dedicated tags that you can use to represent such sections, for example:

- header: **< header>**

- navigation bar: **< nav>**

- main content: **< main>**, with various content subsections represented by **< article>**, **< section>**, and **< div>** elements.

- sidebar: **< aside>**; often placed inside **< main>**

- footer: **< footer>**


# **How does metadata influence Search Engine Optimization?**

Using metadata *boosts your SEO efforts because it's written in the search engine's language.* This helps search engines better understand the topic of your webpages and content. It also helps them display more relevant results to searchers.

# **How is the < meta> HTML tag used when specifying metadata?**

The **< meta>** tag defines metadata about an HTML document. Metadata is data (information) about data. **< meta>** tags always go inside the **< head>** element, and are typically used to specify character set, page description, keywords, author of the document, and viewport settings.


# **What is the first step to designing a Website?**

***How to design a website***

- Set your goal.

- Choose a website builder.

- Define your layout.

- Claim your domain name.

- Gather your content.

- Add the right pages.

- Design your website elements.

- Pick the professional tools you need.

## **Summary**

When starting with a web project, many people focus on the technical side. Of course you must be familiar with the technique of your craft, but what really matters is what you want to *accomplish*.

 Yes, it seems obvious, but too many projects fail not from a lack of technical know-how, but from lack of goals and vision.

*So when you get an idea and want to turn it into a website, there are a few questions you should answer before anything else:*

- What exactly do I want to accomplish?

- How will a website help me reach my goals?

- What needs to be done, and in what order, to reach my goals?

All of this is called *project ideation* and is a necessary first step to reach your goal, whether you are a beginner or an experienced developer.


# **What is the most important question to answer when designing a Website?**

***Who is the website for?***
 One of the most important steps is identifying your ideal audience and anticipated visitors by demographic data, tech-savviness, intent, personal goals and pain point, the stage of their purchase decision making, and more.


# **Why should you use an < h1> element over a < span> element to display a top level heading?**

## **Why would you use the h1 element?**


The H1 tag is an HTML heading that's most commonly used **to mark up a web page title**. Most websites use CSS to make the H1 stand out on the page compared to lesser headings like H2, H3, etc.

In HTML, for example, the **< h1>** element is a semantic element, which gives the text it wraps around the role (or meaning) of "a top level heading on your page."

**Semantic elements
These are some of the roughly 100 semantic elements available:**

- < article>

- < aside>

- < details>

- < figcaption>

- < figure>

- < footer>

- < header>

- < main>

- < mark>

- < nav>

- < section>

- < summary>

- < time>


# **Why Do You Need to Use Semantic Tags in HTML?**

- The semantic HTML tags help the search engines and other user devices to determine the importance and context of web pages.

- The pages made with semantic elements are much easier to read.

- It has greater accessibility. It offers a better user experience.


# **2 Things That Require JavaScript in the Browser**

- Showing and hiding menus or information

- Adding hover effects


# **How can you add JavaScript to an HTML document?**

To include an external JavaScript file, we can **use the script tag with the attribute src**. You've already used the src attribute when using images. The value for the src attribute should be the path to your JavaScript file. This script tag should be included between the **< head>** tags in your HTML document.

