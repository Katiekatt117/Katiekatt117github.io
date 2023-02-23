# **Module 201 Class 3**

## **Boolean**

In *computer science*, a boolean or bool is a *data type* with two possible *values*: **true** or **false**. It is named after the English mathematician and logician **George Boole**, whose algebraic and logical systems are used in all modern digital computers.


### **Tip**

Boolean is pronounced *BOOL-ee-an*. The word "Boolean" should only be capitalized in reference to Boolean logic or Boolean algebra. When referring to the data type in computer programming, the word "boolean" is properly spelled with a lowercase b.


## **HTML: HyperText Markup Language**

**HTML** (HyperText Markup Language) is the most basic building block of the Web. It defines the meaning and structure of web content. Other technologies besides HTML are generally used to describe a web page's appearance/presentation **(CSS)** or functionality/behavior **(JavaScript)**.

"Hypertext" refers to links that connect web pages to one another, either within a single website or between websites. Links are a fundamental aspect of the Web. By uploading content to the Internet and linking it to pages created by other people, you become an active participant in the World Wide Web.

HTML uses "markup" to annotate text, images, and other content for display in a Web browser. HTML markup includes special "elements" such as:

- < head>

- < title>

- < body>

- < header>

- < footer> 

- < article>

- < section>

- < p>

- < div>

- < span>

- < img> 

- < aside> 

- < audio> 

- < canvas> 

- < datalist> 

- < details>

- < embed> 

- < nav>

- < output> 

- < progress

- < video>

- < ul>

- < ol>

- < li>

and many others.

An HTML element is set off from other text in a document by "tags", which consist of the element name surrounded by "<" and ">". The name of an element inside a tag is case insensitive. That is, it can be written in uppercase, lowercase, or a mixture. For example, the **< title>** tag can be written as **< Title>**, **< TITLE>**, or in any other way. However, the convention and recommended practice is to write tags in lowercase.


## **< ol>: The Ordered List element**

The **< ol>** ***HTML*** element represents an ordered list of items — typically rendered as a numbered list.

## **Attributes**

This element also accepts the **global attributes**.


### - **reversed**

This Boolean attribute specifies that the list's items are in reverse order. Items will be numbered from high to low.

### - **start**

An integer to start counting from for the list items. Always an Arabic numeral (1, 2, 3, etc.), even when the numbering type is letters or Roman numerals. For example, to start numbering elements from the letter "d" or the Roman numeral "iv," use **start="4"**.

### - **type**

Sets the numbering type:

- **a** for lowercase letters

- **A** for uppercase letters

- **i** for lowercase Roman numerals

- **I** for uppercase Roman numerals

- **1** for numbers (default)

The specified type is used for the entire list unless a different **type** attribute is used on an enclosed **< li>** element.

### **Note:**

 Unless the type of the list number matters (like legal or technical documents where items are referenced by their number/letter), use the CSS **list-style-type** property instead.


## **Usage notes**

Typically, ordered list items display with a preceding ***marker***, such as a number or letter.

The **< ol>** and **< ul>** elements may nest as deeply as desired, alternating between **< ol>** and **< ul>** however you like.

The **< ol>** and **< ul>** elements both represent a list of items. The difference is with the 
**< ol>** element, the order is meaningful. For example:

- Steps in a recipe

- Turn-by-turn directions

- The list of ingredients in decreasing proportion on nutrition information labels

To determine which list to use, try changing the order of the list items; if the meaning changes, use the **< ol>** element — otherwise you can use **< ul>**.

## **< ul>: The Unordered List element**

The **< ul>** HTML element represents an unordered list of items, typically rendered as a bulleted list.

## **Attributes**

This element includes the ***global attributes***.

- **compact**

This Boolean attribute hints that the list should be rendered in a compact style. The interpretation of this attribute depends on the **user agent**, and it doesn't work in all browsers.

***Warning:***

Do not use this attribute, as it has been deprecated: use ***CSS*** instead. To give a similar effect as the **compact** attribute, the CSS property **line-height** can be used with a value of **80%**.

- **Type**

This attribute sets the bullet style for the list. The values defined under HTML3.2 and the transitional version of HTML 4.0/4.01 are:

- circle

- disc

- square

A fourth bullet type has been defined in the WebTV interface, but not all browsers support it: **triangle**.

If not present and if no **CSS list-style-type** property applies to the element, the user agent selects a bullet type depending on the nesting level of the list.

***Warning:***

 Do not use this attribute, as it has been deprecated; use the **CSS list-style-type** property instead.

Usage notes
The **< ul>** element is for grouping a collection of items that do not have a numerical ordering, and their order in the list is meaningless. Typically, unordered-list items are displayed with a bullet, which can be of several forms, like a dot, a circle, or a square. The bullet style is not defined in the HTML description of the page, but in its associated CSS, using the **list-style-type** property.

The **< ul>** and **< ol>** elements may be nested as deeply as desired. Moreover, the nested lists may alternate between **< ol>** and **< ul>** without restriction.

The **< ol>** and **< ul>** elements both represent a list of items. They differ in that, with the **< ol>** element, the order is meaningful. To determine which one to use, try changing the order of the list items; if the meaning is changed, the **< ol>** element should be used, otherwise you can use **< ul>**.

# **Why do we use an unordered list in HTML?**

An unordered list typically is a bulleted list of items. HTML 3.0 gives you the ability to customise the bullets, to do without bullets and to wrap list items horizontally or vertically for multicolumn lists.

# **How do you change the bullet style of unordered list items?**

How do I change the bullet style in an unordered list?
There are three properties you should know about to start with, which can be set on **< ul>** or **< ol>** elements: list-style-type : Sets the type of bullets to use for the list, for example, square or circle bullets for an unordered list, or numbers, letters, or roman numerals for an ordered list.

# **When should you use an ordered list vs an unorder list in your HTML document?**

An unordered list **( < ul> )** is used to create a list of items in no particular order i.e. the order of items is not relevant. By default, the items in this list will be marked with bullets. Whereas, an ordered list **( < ol> )** is used to create a list of items in a specific order.

# **What are two ways you can change the numbers on list items provided by an ordered list?**

**Type attribute** allows us to change the style of numbers in an ordered list. Explanation: The < li > tag includes two attributes – type and value. The type attribute is used to modify the order numbering in the list item.

# **Learn CSS**

Cascading Style Sheets — or **CSS** — is the first technology you should start learning after **HTML**. While HTML is used to define the structure and semantics of your content, CSS is used to style it and lay it out. For example, you can use CSS to alter the font, color, size, and spacing of your content, split it into multiple columns, or add animations and other decorative features.

# **Prerequisites**

You should learn the basics of HTML before attempting any CSS. We recommend that you work through our Introduction to HTML module first.

CSS (Cascading Style Sheets) is used to style and layout web pages — for example, to alter the font, color, size, and spacing of your content, split it into multiple columns, or add animations and other decorative features. This module provides a gentle beginning to your path towards CSS mastery with the basics of how it works, what the syntax looks like, and how you can start using it to add styling to HTML.

Everything in CSS has a box around it, and understanding these boxes is key to being able to create more complex layouts with CSS, or to align items with other items.

# **Block and inline boxes**

In CSS we have several types of boxes that generally fit into the categories of block boxes and inline boxes. The type refers to how the box behaves in terms of page flow and in relation to other boxes on the page. Boxes have an inner display type and an outer display type.

In general, you can set various values for the display type using the **display** property, which can have various values.

# **Outer display type**

If a box has an outer display type of **block**, then:

- The box will break onto a new line.

- The **width** and **height** properties are respected.

- Padding, margin and border will cause other elements to be pushed away from the box.

- If **width** is not specified, the box will extend in the inline direction to fill the space available in its container. In most cases, the box will become as wide as its container, filling up 100% of the space available.

Some HTML elements, such as **< h1>** and **< p>**, use block as their outer display type by default.

If a box has an outer display type of **inline**, then:

- The box will not break onto a new line.

- The **width** and **height** properties will not apply.

- Vertical padding, margins, and borders will apply but will not cause other inline boxes to move away from the box.

- Horizontal padding, margins, and borders will apply and will cause other inline boxes to move away from the box.

Some HTML elements, such as **< a>**, **< span>**, **< em>** and **< strong>** use **inline** as their outer display type by default.

# **Inner display type**

Boxes also have an *inner* display type, which dictates how elements inside that box are laid out.

Block and inline layout is the default way things behave on the web. By default and without any other instruction, the elements inside a box are also laid out in **normal flow** and behave as block or inline boxes.

You can change the inner display type for example by setting **display: flex**;. The element will still use the outer display type **block** but this changes the inner display type to **flex**. Any direct children of this box will become flex items and behave according to the Flexbox specification.

When you move on to learn about CSS Layout in more detail, you will encounter **flex**, and various other inner values that your boxes can have, for example **grid**.

# **What data types can you store inside of an Array?**

Arrays are classified as Homogeneous Data Structures because they store elements of the same type. They can store **numbers**, **strings**, **boolean values** **(true and false)**, **characters**, **objects**, and so on. But once you define the type of values that your array will store, all its elements must be of that same type.

# **Five shorthand operators for assignment in javascript**

- Assignment

	x = f()	x = f()

- Addition assignment

  x += f()	x = x + f()

- Subtraction assignment

	x -= f()	x = x - f()

- Multiplication assignment

	x *= f()	x = x * f()
- Division assignment

    x /= f()	x = x / f

# **What is an example of a conditional statement in programming?**

In programming, a great example of a condition is a **password**.

 Passwords are “if, then” logic statements: If a user enters the correct password, then they can access the program.

# **An example of when a Loop is useful in JavaScript**

In programming, loops are used to repeat a block of code. For example, if you want to show a message 100 times, then you can use a loop.