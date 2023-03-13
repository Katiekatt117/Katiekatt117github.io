# **Creating hyperlinks**

Hyperlinks are really important — they are what makes the Web a web.

# **What is a hyperlink?**

Hyperlinks are one of the most exciting innovations the Web has to offer. They've been a feature of the Web since the beginning, and are what makes the Web a web. Hyperlinks allow us to link documents to other documents or resources, link to specific parts of documents, or make apps available at a web address. Almost any web content can be converted to a link so that when clicked or otherwise activated the web browser goes to another web address **(URL)**.

**Note:**
 A URL can point to HTML files, text files, images, text documents, video and audio files, or anything else that lives on the Web. If the web browser doesn't know how to display or handle the file, it will ask you if you want to open the file (in which case the duty of opening or handling the file is passed to a suitable native app on the device) or download the file (in which case you can try to deal with it later on).

For example, the BBC homepage contains many links that point not only to multiple news stories, but also different areas of the site (navigation functionality), login/registration pages (user tools), and more.

# **Anatomy of a link**

A basic link is created by wrapping the text or other content inside an **< a>** element and using the href attribute, also known as a Hypertext Reference, or target, that contains the web address.

# **Block level links**

As mentioned before, almost any content can be made into a link, even ***block-level elements***. If you want to make a heading element a link then wrap it in an anchor **(< a>)** element 

# **Image links**

If you have an image you want to make into a link, use the **< a>** element to wrap the image file referenced with the **< img>** element.

# **Adding supporting information with the title attribute**

Another attribute you may want to add to your links is title. The title contains additional information about the link, such as which kind of information the page contains, or things to be aware of on the website.

**Note:** A link title is only revealed on mouse hover, which means that people relying on keyboard controls or touchscreens to navigate web pages will have difficulty accessing title information. If a title's information is truly important to the usability of the page, then you should present it in a manner that will be accessible to all users, for example by putting it in the regular text.

# **URLs and paths**

A URL, or Uniform Resource Locator is a string of text that defines where something is located on the Web. For example, Mozilla's English homepage is located at ***https://www.mozilla.org/en-US/***.

URLs use paths to find files. Paths specify where the file you're interested in is located in the filesystem. 

The root of this directory structure is called creating-hyperlinks. When working locally with a website, you'll have one directory that contains the entire site. Inside the root, we have an index.html file and a contacts.html. In a real website, index.html would be our home page or landing page (a web page that serves as the entry point for a website or a particular section of a website.).

There are also two directories inside our root — pdfs and projects. These each have a single file inside them — a PDF (project-brief.pdf) and an index.html file, respectively. Note that you can have two index.html files in one project, as long as they're in different filesystem locations. The second index.html would perhaps be the main landing page for project-related information.

# **Same directory:**

If you wanted to include a hyperlink inside index.html (the top level index.html) pointing to contacts.html, you would specify the filename that you want to link to, because it's in the same directory as the current file. The URL you would use is contacts.html

# **Moving down into subdirectories:**

If you wanted to include a hyperlink inside index.html (the top level index.html) pointing to projects/index.html, you would need to go down into the projects directory before indicating the file you want to link to. This is done by specifying the directory's name, then a forward slash, then the name of the file. The URL you would use is projects/index.html

**Note:** You can combine multiple instances of these features into complex URLs, if needed, for example: ***../../../complex/path/to/my/file.html***.

# **Document fragments**

It's possible to link to a specific part of an HTML document, known as a document fragment, rather than just to the top of the document. To do this you first have to assign an id attribute to the element you want to link to. 

Then to link to that specific id, you'd include it at the end of the URL, preceded by a hash/pound symbol **(#)**

# **Absolute versus relative URLs**

Two terms you'll come across on the Web are absolute URL and relative URL:

- **absolute URL:**
 Points to a location defined by its absolute location on the web, including protocol and domain name. For example, if an index.html page is uploaded to a directory called projects that sits inside the root of a web server, and the website's domain is ***https://www.example.com***, the page would be available at ***https://www.example.com/projects/index.html*** (or even just ***https://www.example.com/projects/***, as most web servers just look for a landing page such as index.html to load if it isn't specified in the URL.)

An absolute URL will always point to the same location, no matter where it's used.

- **relative URL:**
Points to a location that is relative to the file you are linking from, more like what we looked at in the previous section. For example, if we wanted to link from our example file at ***https://www.example.com/projects/index.html*** to a PDF file in the same directory, the URL would just be the filename — **project-brief.pdf** — no extra information needed. If the PDF was available in a subdirectory inside projects called pdfs, the relative link would be pdfs/project-brief.pdf (the equivalent absolute URL would be ***https://www.example.com/projects/pdfs/project-brief.pdf.)***

A relative URL will point to different places depending on the actual location of the file you refer from — for example if we moved our index.html file out of the projects directory and into the root of the website (the top level, not in any directories), the pdfs/project-brief.pdf relative URL link inside it would now point to a file located at ***https://www.example.com/pdfs/project-brief.pdf***, not a file located at ***https://www.example.com/projects/pdfs/project-brief.pdf***.

Of course, the location of the project-brief.pdf file and pdfs folder won't suddenly change because you moved the index.html file — this would make your link point to the wrong place, so it wouldn't work if clicked on.


# **To create a basic link, we wrap text or other content inside what element?**

A basic link is created by wrapping the text or other content inside an **< a>** element and using the href attribute, also known as a Hypertext Reference, or target, that contains the web address.

**The href attribute contains what information?**

For **< link>** elements, the href attribute specifies the location (URL) of the external resource (most often a style sheet file).

# **What are some ways we can ensure links on our pages are accessible to all readers?**

- Create Accessible Hypertext Links

- Use concise and meaningful text for links.

- Do not capitalize all letters in links.

- Avoid using URLs for link text.

- Do not use the word "link" as part of the link text.

- Do not use tooltips/screentips to add additional information.

# **CSS Normal Flow**

As detailed in the last lesson introducing layout, elements on a webpage lay out in normal flow if you haven't applied any CSS to change the way they behave. And, as we began to discover, you can change how elements behave either by adjusting their position in normal flow or by removing them from it altogether. Starting with a solid, well-structured document that's readable in normal flow is the best way to begin any webpage. It ensures that your content is readable even if the user's using a very limited browser or a device such as a screen reader that reads out the content of the page. In addition, since normal flow is designed to make a readable document, by starting in this way you're working with the document rather than struggling against it as you make changes to the layout.


# **How are elements laid out by default?**

The process begins as the boxes of individual elements are laid out in such a way that any padding, border, or margin they happen to have is added to their content. This is what we call the box model.

By default, a block level element's content fills the available inline space of the parent element containing it and the element grows along the block dimension to accommodate its content. The size of inline elements is just the size of their content. You can't set width or height on inline elements — they just sit inside the content of block level elements — except for images. Unlike other inline elements, images can be resized without changing their display property. If you want to control the size of an inline element in this manner, you need to set it to behave like a block level element (e.g., with display: block; or display: inline-block;, which mixes characteristics from both).

That explains how elements are structured individually, but how about the way they're structured when they interact with one another? The normal layout flow (mentioned in the layout introduction article) is the system by which elements are placed inside the browser's viewport. By default, block-level elements are laid out in the block flow direction, which is based on the parent's writing mode (initial: horizontal-tb). Each element will appear on a new line below the last one, with each one separated by whatever margin that's been specified. 

***In English, for example, (or any other horizontal, top to bottom writing mode) block-level elements are laid out vertically.***

*Inline elements behave differently.*

They don't appear on new lines; instead, they all sit on the same line along with any adjacent (or wrapped) text content as long as there is space for them to do so inside the width of the parent block level element. If there isn't space, then the overflowing content will move down to a new line.

If two vertically adjacent elements both have a margin set on them and their margins touch, the larger of the two margins remains and the smaller one disappears. This is known as **margin collapsing**. Collapsing margins is only relevant in the *vertical direction*.

## **Summary**

In this lesson you've learned the basics of normal flow — the default layout for CSS elements. By understanding how inline elements, block elements, and margins behave by default, it'll be easier to modify their behavior in the future.

# **Positioning**

Positioning allows you to take elements out of normal document flow and make them behave differently, for example, by sitting on top of one another or by always remaining in the same place inside the browser viewport. This article explains the different position values and how to use them.

## **Introducing positioning**

Positioning allows us to produce interesting results by overriding normal document flow. What if you want to slightly alter the position of some boxes from their default flow position to give a slightly quirky, distressed feel? Positioning is your tool. Or what if you want to create a UI element that floats over the top of other parts of the page and/or always sits in the same place inside the browser window no matter how much the page is scrolled? Positioning makes such layout work possible.

There are a number of different types of positioning that you can put into effect on HTML elements. *To make a specific type of positioning active on an element, we use the position property*.

# **Static positioning**

Static positioning is the default that every element gets. It just means *"put the element into its normal position in the document flow — nothing special to see here."*

To see this (and get your example set up for future sections) first add a class of positioned to the second **< p>** in the HTML

If you save and refresh, you'll see no difference at all, except for the updated background color of the 2nd paragraph. This is fine — as we said before, static positioning is the default behavior!

# **Static positioning**

Static positioning is the default that every element gets. It just means *"put the element into its normal position in the document flow — nothing special to see here."*

To see this (and get your example set up for future sections) first add a class of positioned to the second **< p>** in the HTML:

- < p class="positioned">…< /p>


Now add the following rule to the bottom of your CSS:

- .positioned {
  position: static;
  background: yellow;
- }

If you save and refresh, you'll see no difference at all, except for the updated background color of the 2nd paragraph. This is fine — as we said before, static positioning is the default behavior!

**Note:** You can see the example at this point live at ***1_static-positioning.html*** (see source code).

# **Relative positioning**

Relative positioning is the first position type we'll take a look at. This is very similar to static positioning, except that once the positioned element has taken its place in the normal flow, you can then modify its final position, including making it overlap other elements on the page. Go ahead and update the position declaration in your code:

- position: relative;

If you save and refresh at this stage, you won't see a change in the result at all. So how do you modify the element's position? You need to use the top, bottom, left, and right properties, which we'll explain in the next section.

Introducing top, bottom, left, and right
top, bottom, left, and right are used alongside position to specify exactly where to move the positioned element to. To try this out, add the following declarations to the .positioned rule in your CSS:

- top: 30px;

- left: 30px;

**Note:** The values of these properties can take any units you'd reasonably expect: pixels, mm, rems, %, etc.

# **What is meant by “normal flow”?**

Normal Flow, or Flow Layout, is the way that Block and Inline elements are displayed on a page before any changes are made to their layout. The flow is essentially a set of things that are all working together and know about each other in your layout. Once something is taken out of flow it works independently.

# **What are a few differences between block-level and inline elements?**

Block elements always start from a new line. Inline elements never start from a new line. Block elements cover space from left to right as far as it can go. Inline elements only cover the space as bounded by the tags in the HTML element.

**STATIC** positioning is the default for every html element.

HTML elements are positioned static by default. Static positioned elements are not affected by the top, bottom, left, and right properties.

# **What are a few advantages to using absolute positioning on an element?**

Some of the benefits of using absolutely positioned elements in your layouts include:
Aside from a few IE bugs, very good cross-browser support.
Less dependence on floats, which can be problematic.
Less dependence on margins, which can be a bit buggy in older IE.

# **What is a key difference between fixed positioning and absolute positioning?**

Absolutely positioned elements are positioned with respect to a containing block, which is the nearest postioned ancestor. If there is no positioned ancestor, the viewport will be the containing block. Elements with fixed positioning are fixed with respect to the viewport—the viewport is always their containing block.


# **Functions — reusable blocks of code**

Another essential concept in coding is functions, which allow you to store a piece of code that does a single task inside a defined block, and then call that code whenever you need it using a single short command — rather than having to type out the same code multiple times. In this article we'll explore fundamental concepts behind functions such as basic syntax, how to invoke and define them, scope, and parameters.

# **Where do I find functions?**

In JavaScript, you'll find functions everywhere. In fact, we've been using functions all the way through the course so far; we've just not been talking about them very much. Now is the time, however, for us to start talking about functions explicitly, and really exploring their syntax.

Pretty much anytime you make use of a JavaScript structure that features a pair of parentheses — () — and you're not using a common built-in language structure like a for loop, while or do...while loop, or if...else statement, you are making use of a function.

The JavaScript language has many built-in functions to allow you to do useful things without having to write all that code yourself. In fact, some of the code you are calling when you invoke (a fancy word for run, or execute) a built in browser function couldn't be written in JavaScript — many of these functions are calling parts of the background browser code, which is written largely in low-level system languages like C++, not web languages like JavaScript.

Bear in mind that some built-in browser functions are not part of the core JavaScript language — some are defined as part of browser APIs, which build on top of the default language to provide even more functionality (refer to this early section of our course for more descriptions). We'll look at using browser APIs in more detail in a later module.

# **Functions versus methods**

Functions that are part of objects are called methods. You don't need to learn about the inner workings of structured JavaScript objects yet — you can wait until our later module that will teach you all about the inner workings of objects, and how to create your own. For now, we just wanted to clear up any possible confusion of method versus function — you are likely to meet both terms as you look at the available related resources across the Web.

The built-in code we've made use of so far come in both forms: functions and methods. You can check the full list of the built-in functions, as well as the built-in objects and their corresponding methods here.

You've also seen a lot of custom functions in the course so far — functions defined in your code, not inside the browser. Anytime you saw a custom name with parentheses straight after it, you were using a custom function. In our random-canvas-circles.html example (see also the full source code) from our loops article, we included a custom draw() function

This function draws 100 random circles inside a **< canvas>** element. Every time we want to do that, we can just invoke the function with this:

- draw();

rather than having to write all that code out again every time we want to repeat it. And functions can contain whatever code you like — you can even call other functions from inside functions. The above function for example calls the random() function three times

# **Invoking functions**

You are probably clear on this by now, but just in case, to actually use a function after it has been defined, you've got to run — or invoke — it. This is done by including the name of the function in the code somewhere, followed by parentheses.

Note: This form of creating a function is also known as function declaration. It is always hoisted, so you can call function above function definition and it will work fine.

# **Function parameters**

Some functions require parameters to be specified when you are invoking them — these are values that need to be included inside the function parentheses, which it needs to do its job properly.

**Note:** Parameters are sometimes called arguments,

# **Optional parameters**

Sometimes parameters are optional — you don't have to specify them. If you don't, the function will generally adopt some kind of default behavior. As an example, the array join() function's parameter is optional

If no parameter is included to specify a joining/delimiting character, a comma is used by default.

# **Default parameters**

If you're writing a function and want to support optional parameters, you can specify default values by adding = after the name of the parameter, followed by the default value

# **Anonymous function example**

For example, let's say you want to run some code when the user types into a text box. To do this you can call the addEventListener() function of the text box. This function expects you to pass it (at least) two parameters:

the name of the event to listen for, which in this case is keydown
a function to run when the event happens.
When the user presses a key, the browser will call the function you provided, and will pass it a parameter containing information about this event, including the particular key that the user pressed

Instead of defining a separate logKey() function, you can pass an anonymous function into addEventListener()

Arrow functions
If you pass an anonymous function like this, there's an alternative form you can use, called an arrow function. Instead of function(event), you write (event) =>


# **Describe the difference between a function declaration and a function invocation.**

A function expression is very similar to and has almost the same syntax as a function declaration (see function statement for details). The main difference between a function expression and a function declaration is the function name, which can be omitted in function expressions to create anonymous functions.

# **What is the difference between a parameter and an argument?**

**Argument Vs. Parameter:** 

Explore the Major Difference between Argument and Parameter. The values that are declared within a function when the function is called are known as an argument. Whereas, the variables that are defined when the function is declared are known as a parameter.