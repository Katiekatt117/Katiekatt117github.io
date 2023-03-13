# **Domain Modeling**

Domain modeling is the process of creating a conceptual model in code for a specific problem. A model describes the various entities, their attributes and behaviors, as well as the constraints that govern the problem domain. An entity that stores data in properties and encapsulates behaviors in methods is commonly referred to as an ***object-oriented model***.

A domain model that's articulated well can verify and validate the understanding of a specific problem among various stakeholders. As a communication tool, it defines a vocabulary that can be used within and between both technical and business teams.

# **Model epic fails videos**

Imagine you've been tasked to build a program that models the popularity of epic fail videos. After months of painstaking research, you've determined that the two essential metrics for gauging popularity are an epic rating and whether or not the video has animals.

Since you'll be modeling the popularity of many types of videos—parkour epic fails, corgi epic fails, etc.—you'll want to build self-contained objects with the same attributes and behaviors. That way, when you need to change the algorithm for determining popularity, the changes will be small and targeted.

To define the same properties between many objects, you'll want to use a constructor function.

As you can see, the constructor function is defined using a function expression. In other words, the variable **EpicFailVideo** is declared and then assigned a function with two parameters called **epicRating** and **hasAnimals**.

When the function is called, the data inside these parameters are stored inside the **this.epicRating** and **this.hasAnimals** properties respectively. Storing data within properties ensures any newly created object can access that data later.

After the constructor function definition, two objects are instantiated with the **new** keyword and their properties are initialized by calling the **EpicFailVideo** constructor function. After being instantiated and initialized, these objects are stored inside the **parkourFail** and **corgiFail** variables.

This is **object-oriented programming** in JavaScript at its most fundamental level.

1.) The new keyword instantiates (i.e. creates) an object.

2.) The constructor function initializes properties inside that object using the this variable.

3.) The object is stored in a variable for later use.

# **Generate random numbers**

To model the random nature of user behavior, you'll need the help of a random number generator. Fortunately, the JavaScript standard library includes a **Math.random()** function for just this sort of occasion.

**EpicFailVideo**'s prototype is given a **generateRandom** method which is assigned a function with two parameters called **min** and **max**. The function uses both **Math.floor** and **Math.random** to calculate and return a random integer between **min** and **max**.

When **parkourFail** is asked to run the **generateRandom()** method, it searches through all of its own methods. When it doesn't find the **generateRandom()** method there, **parkourFail** then searches through all of the methods on its prototype object. When it finds the **generateRandom()** method on its prototype object, **parkourFail** calls the method, passing in 1 and 5 as the arguments. The **generateRandom(1, 5)** method runs and returns a random number between **1** and **5**. The exact same process happens for **corgiFail** too.

While it certainly takes longer to locate a method on the prototype object, this technique is an established best practice in JavaScript. When a prototype is shared between two or more objects, like it is for **parkourFail** and **corgiFail**, those objects execute the same code when the **generateRandom()** method is called. And shared code means a running program consumes less memory which is important for devices like smart phones and tablets.

# **HTML table basics**

## **What is a table?**

A ***table*** is a structured set of data made up of rows and columns **(tabular data)**. A table allows you to quickly and easily look up values that indicate some kind of connection between different types of data, for example a person and their age, or a day of the week, or the timetable for a local swimming pool.

# **How does a table work?**

The point of a table is that it is rigid. Information is easily interpreted by making visual associations between row and column headers. Look at the table below for example and find a Jovian gas giant with 62 moons. You can find the answer by associating the relevant row and column headers.

When implemented correctly, HTML tables are handled well by accessibility tools such as screen readers, so a successful HTML table should enhance the experience of sighted and visually impaired users alike.

# **Table styling**

You can also have a look at the live example on GitHub! One thing you'll notice is that the table does look a bit more readable there — this is because the table you see above on this page has minimal styling, whereas the GitHub version has more significant CSS applied.

Be under no illusion; for tables to be effective on the web, you need to provide some styling information with **CSS**, as well as good solid structure with HTML.

# **When should you NOT use HTML tables?**

HTML tables should be used for tabular data — this is what they are designed for. Unfortunately, a lot of people used to use HTML tables to lay out web pages, e.g. one row to contain the header, one row to contain the content columns, one row to contain the footer, etc. You can find more details and an example at Page Layouts in our Accessibility Learning Module. This was commonly used because CSS support across browsers used to be terrible; table layouts are much less common nowadays, but you might still see them in some corners of the web.

In short, using tables for layout rather than CSS layouttechniques is a bad idea. The main reasons are as follows:

1.) **Layout tables reduce accessibility for visually impaired users:** screen readers, used by blind people, interpret the tags that exist in an HTML page and read out the contents to the user. Because tables are not the right tool for layout, and the markup is more complex than with CSS layout techniques, the screen readers' output will be confusing to their users.

2.) **Tables produce tag soup:** As mentioned above, table layouts generally involve more complex markup structures than proper layout techniques. This can result in the code being harder to write, maintain, and debug.

3.) **Tables are not automatically responsive:** When you use proper layout containers (such as **< header>**, **< section>**, **< article>**, or **< div>**), their width defaults to 100% of their parent element. Tables on the other hand are sized according to their content by default, so extra measures are needed to get table layout styling to effectively work across a variety of devices.

# **Adding headers with < th> elements**

Now let's turn our attention to table headers — special cells that go at the start of a row or column and define the type of data that row or column contains

# **Why are headers useful?**

We have already partially answered this question — it is easier to find the data you are looking for when the headers clearly stand out, and the design just generally looks better.

**Note:** Table headings come with some default styling — they are bold and centered even if you don't add your own styling to the table, to help them stand out.

Tables headers also have an added benefit — along with the **scope** attribute (which we'll learn about in the next article), they allow you to make tables more accessible by associating each header with all the data in the same row or column. Screen readers are then able to read out a whole row or column of data at once, which is pretty useful.

# **Styling without < col>**

There is one last feature we'll tell you about in this article before we move on. HTML has a method of defining styling information for an entire column of data all in one place — the **< col>** and **< colgroup>** elements. These exist because it can be a bit annoying and inefficient having to specify styling on columns — you generally have to specify your styling information on every **< td>** or **< th>** in the column, or use a complex selector such as **:nth-child**.

**Note:** Styling columns like this is limited to a few properties: **border**, **background**, **width**, and **visibility**. To set other properties you'll have to either style every **< td>** or **< th>** in the column, or use a complex selector such as **:nth-child**.

Styling with **< col>**
Instead of doing this, we can specify the information once, on a **< col>** element. **< col>** elements are specified inside a **< colgroup>** container just below the opening **< table>** tag. 

Just like **colspan** and **rowspan**, **span** takes a unitless number value that specifies the number of columns you want the styling to apply to.


# **Why do we need domain modeling?**

Domain modeling is a great tool for Agile enterprise to carry out a common language and a fundamental structure important for the analysis of features and epics. The domain model is defined and continuously refactored as enterprise knowledge about the domain improves and the system functionality evolves.

# **Why should tables not be used for page layouts?**

HTML tables were originally intended to be used for presenting tabular data, not for layout. The World Wide Web Consortium (W3C®) discourages use of tables for layout because they are striving for a web in which content and structure are completely separate from presentation.

# **3 different semantic HTML elements used in an HTML < table>.**

Examples of semantic elements: < form> , < table> , and < article>

# **What is a constructor and what are some advantages to using it?**

Constructors are methods that are automatically executed every time you create an object. The purpose of a constructor is to construct an object and assign values to the object's members. A constructor takes the same name as the class to which it belongs, and does not return any values.

# **How does the term this differ when used in an object literal versus when used in a constructor?**

Objects created using object literal are singletons, this means when a change is made to the object, it affects the object entire the script. Whereas if an object is created using constructor function and a change is made to it, that change won't affect the object throughout the script.

# **What are prototype methods in javascript?**

A prototype is an existing inbuilt functionality in JavaScript. Whenever we create a JavaScript function, JavaScript adds a prototype property to that function. A prototype is an object, where it can add new variables and methods to the existing object.