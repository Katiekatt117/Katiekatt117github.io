# **HTML**

One of HTML's main jobs is to give text structure so that a browser can display an HTML document the way its developer intends. This article explains the way HTML can be used to structure a page of text by adding headings and paragraphs, emphasizing words, creating lists, and more.

Most structured text consists of headings and paragraphs, whether you are reading a story, a newspaper, a college textbook, a magazine, etc.

Structured content makes the reading experience easier and more enjoyable.

In HTML, each paragraph has to be wrapped in a **< p>** element, like so:

- **< p>**I am a paragraph, oh yes I am.**< /p>**

Each heading has to be wrapped in a heading element:

- **< h1>**I am the title of the story.**< /h1>**

There are six heading elements: **h1**, **h2**, **h3**, **h4**, **h5**, and **h6**. Each element represents a different level of content in the document; **< h1>** represents the main heading, **< h2>** represents subheadings, **< h3>** represents sub-subheadings, and so on.

- Preferably, you should use a single **< h1>** per page—this is the top level heading, and all others sit below this in the hierarchy.

- Make sure you use the headings in the correct order in the hierarchy. Don't use **< h3>** elements to represent subheadings, followed by **< h2>** elements to represent sub-subheadings—that doesn't make sense and will lead to weird results.

- Of the six heading levels available, you should aim to use no more than three per page, unless you feel it is necessary. Documents with many levels (for example, a deep heading hierarchy) become unwieldy and difficult to navigate. On such occasions, it is advisable to spread the content over multiple pages if possible.

# **description lists**

The purpose of these lists is to mark up a set of items and their associated descriptions, such as terms and definitions, or questions and answers.

Description lists use a different wrapper than the other list types — **< dl>**; in addition each term is wrapped in a **< dt>** (description term) element, and each description is wrapped in a **< dd>** (description definition) element.

# **Why is it important to use semantic elements in our HTML?**

Writing semantic HTML makes your code easier to understand, making the source code more readable for other developers. Screen readers and browsers can interpret Semantic HTML better, which makes it more accessible.

# **How many levels of headings are there in HTML?**

6 read above to find out what they are

# **What are some uses for the < sup> and < sub> elements?**

The sup element represents a superscript and the sub element represents a subscript. These elements must be used only to mark up typographical conventions with specific meanings, not for typographical presentation for presentation's sake.

# **When using the < abbr> element, what attribute must be added to provide the full expansion of the term?**

The title attribute may be used to provide an expansion of the abbreviation. The attribute, if specified, must contain an expansion of the abbreviation, and nothing else.

# **CSS**

An external stylesheet contains CSS in a separate file with a .css extension. This is the most common and useful method of bringing CSS to a document. You can link a single CSS file to multiple web pages, styling all of them with the same CSS stylesheet. In the Getting started with CSS, we linked an external stylesheet to our web page.

An internal stylesheet resides within an HTML document. To create an internal stylesheet, you place CSS inside a **< style>** element contained inside the HTML **< head>**.

For sites with more than one page, an internal stylesheet becomes a less efficient way of working. To apply uniform CSS styling to multiple pages using internal stylesheets, you must have an internal stylesheet in every web page that will use the styling. The efficiency penalty carries over to site maintenance too. With CSS in internal stylesheets, there is the risk that even one simple styling change may require edits to multiple web pages.

Inline styles are CSS declarations that affect a single HTML element, contained within a style attribute.

# **What are ways we can apply CSS to your HTML?**

## **CSS can be added to HTML documents in 3 ways:**

1.) Inline - by using the style attribute inside HTML elements.

2.) Internal - by using a < style> element in the < head> section.

3.) External - by using a < link> element to link to an external CSS file.

# **Why should we avoid using inline styles?**

One of the main reasons that inline styling is not a good choice for your application is because it does not support (or it has really poor support) for CSS features. Every application nowadays might have to end up using some selectors such as :hover , :active , :focused , etc.

