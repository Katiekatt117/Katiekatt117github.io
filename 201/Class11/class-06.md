# **JavaScript object basics**

An object is a collection of related data and/or functionality. These usually consist of several variables and functions (which are called properties and methods when they are inside objects). Let's work through an example to understand what they look like.

To begin with, make a local copy of our oojs.html file. This contains very little — a **< script>** element for us to write our source code into. We'll use this as a basis for exploring basic object syntax. While working with this example you should have your developer tools JavaScript console open and ready to type in some commands.

***As with many things in JavaScript, creating an object often begins with defining and initializing a variable.***

**So what is going on here?** Well, an object is made up of multiple members, each of which has a name (e.g. name and age above), and a value (e.g. ['Bob', 'Smith'] and 32). Each name/value pair must be separated by a comma, and the name and value in each case are separated by a colon.

The value of an object member can be pretty much anything — in our person object we've got a number, an array, and two functions. The first two items are data items, and are referred to as the object's properties. The last two items are functions that allow the object to do something with that data, and are referred to as the object's methods.

It is very common to create an object using an object literal when you want to transfer a series of structured, related data items in some manner, for example sending a request to the server to be put into a database. Sending a single object is much more efficient than sending several items individually, and it is easier to work with than an array, when you want to identify individual items by name.

# **Dot notation**

Above, you accessed the object's properties and methods using dot notation. The object name (person) acts as the namespace — it must be entered first to access anything inside the object. Next you write a dot, then the item you want to access — this can be the name of a simple property, an item of an array property, or a call to one of the object's methods.

***An object property can itself be an object.***

# **Bracket notation**

Bracket notation provides an alternative way to access object properties. Instead of using dot notation, You can instead use brackets.

This looks very similar to how you access the items in an array, and it is basically the same thing — instead of using an index number to select an item, you are using the name associated with each member's value. It is no wonder that objects are sometimes called associative arrays — they map strings to values in the same way that arrays map numbers to values.

Dot notation is generally preferred over bracket notation because it is more succinct and easier to read. However there are some cases where you have to use brackets. For example, if an object property name is held in a variable, then you can't use dot notation to access the value, but you can access the value using bracket notation.

# **Setting object members**

So far we've only looked at retrieving (or getting) object members — you can also set (update) the value of object members by declaring the member you want to set (using dot or bracket notation)

Setting members doesn't just stop at updating the values of existing properties and methods; you can also create completely new members.

One useful aspect of bracket notation is that it can be used to set not only member values dynamically, but member names too. Let's say we wanted users to be able to store custom value types in their people data, by typing the member name and value into two text inputs.

# **What is "this"?**

You are probably wondering what **"this"** is. The **this** keyword refers to the current object the code is being written inside — so in this case this is equivalent to person. So why not just write person instead?

Well, when you only have to create a single object literal, it's not so useful. But if you create more than one, this enables you to use the same method definition for every object you create.

# **Introducing constructors**

Using object literals is fine when you only need to create one object, but if you have to create more than one, as in the previous section, they're seriously inadequate. We have to write out the same code for every object we create, and if we want to change some properties of the object - like adding a height property - then we have to remember to update every object.

We would like a way to define the **"shape"** of an object — the set of methods and the properties it can have — and then create as many objects as we like, just updating the values for the properties that are different.

Constructors, by convention, start with a capital letter and are named for the type of object they create.

# **Introduction to the DOM**

The ***Document Object Model (DOM)*** is the data representation of the objects that comprise the structure and content of a document on the web. This guide will introduce the DOM, look at how the DOM represents an HTML document in memory and how to use APIs to create web content and applications.

# **What is the DOM?**

The ***Document Object Model (DOM)*** is a programming interface for web documents. It represents the page so that programs can change the document structure, style, and content. The DOM represents the document as nodes and objects; that way, programming languages can interact with the page.

A web page is a document that can be either displayed in the browser window or as the HTML source. In both cases, it is the same document but the ***Document Object Model (DOM)*** representation allows it to be manipulated. As an object-oriented representation of the web page, it can be modified with a scripting language such as JavaScript.

For example, the ***DOM*** specifies that the querySelectorAll method in this code snippet must return a list of all the **< p>** elements in the document

All of the properties, methods, and events available for manipulating and creating web pages are organized into objects. For example, the document object that represents the document itself, any table objects that implement the **HTMLTableElement DOM** interface for accessing HTML tables, and so forth, are all objects.

The ***DOM*** is built using multiple APIs that work together. The core ***DOM*** defines the entities describing any document and the objects within it. This is expanded upon as needed by other ***APIs*** that add new features and capabilities to the ***DOM***. For example, the ***HTML DOM API*** adds support for representing HTML documents to the core ***DOM***, and the SVG API adds support for representing SVG documents.

# **DOM and JavaScript**

The previous short example, like nearly all examples, is JavaScript. That is to say, it is written in JavaScript, but uses the DOM to access the document and its elements. The DOM is not a programming language, but without it, the JavaScript language wouldn't have any model or notion of web pages, HTML documents, SVG documents, and their component parts. The document as a whole, the head, tables within the document, table headers, text within the table cells, and all other elements in a document are parts of the document object model for that document. They can all be accessed and manipulated using the DOM and a scripting language like JavaScript.

***The DOM is not part of the JavaScript language, but is instead a Web API used to build websites.***

 JavaScript can also be used in other contexts. For example, Node.js runs JavaScript programs on a computer, but provides a different set of APIs, and the DOM API is not a core part of the Node.js runtime.

The DOM was designed to be independent of any particular programming language, making the structural representation of the document available from a single, consistent API. Even if most web developers will only use the DOM through JavaScript, implementations of the DOM can be built for any language

# **Accessing the DOM**

You don't have to do anything special to begin using the DOM. You use the API directly in JavaScript from within what is called a script, a program run by a browser.

When you create a script, whether inline in a **< script>** element or included in the web page, you can immediately begin using the API for the document or window objects to manipulate the document itself, or any of the various elements in the web page (the descendant elements of the document). Your DOM programming may be something as simple as the following example, which displays a message on the console by using the console.log() function

As it is generally not recommended to mix the structure of the page (written in HTML) and manipulation of the DOM (written in JavaScript), the JavaScript parts will be grouped together here, and separated from the HTML.

# **What is an Object in java?**

In the Java programming language, an object is an instance of a Java class, meaning it is a copy of a specific class. Java objects have three primary characteristics: identity, state, and behavior. These characteristics are the building blocks of any class object and set the scene for how they are used.


# **What are some advantages to creating object literals?**

The advantages of using object literals to create objects include convenience, flexibility in declaration, and less code during declaration. You can drop an object literal anywhere in your program with no previous setup and it'll work, which can be very handy!


# **How do objects differ from arrays?**

Objects represent “things” with characteristics (aka properties), while arrays create and store lists of data in a single variable.


# **Example for when you would need to use bracket notation to access an object’s property instead of dot notation.**

dot notation is the most common way to access elements in JavaScript. However, there are certain situations where bracket notation is more appropriate. When you want to use a variable to access a property, or if a property has special characters in its name, you should use bracket notation.

