# **Images in HTML**

There are other types of multimedia to consider, but it is logical to start with the humble **< img>** element, used to embed a simple image in a webpage. In this article we'll look at how to use it in depth, including the basics, annotating it with captions using **< figure>**, and detailing how it relates to CSS background images.

# **How do we put an image on a webpage?**

In order to put a simple image on a web page, we use the **< img>** element. This is a void element (meaning, it cannot have any child content and cannot have an end tag) that requires two attributes to be useful: src and alt. The src attribute contains a URL pointing to the image you want to embed in the page. As with the href attribute for **< a>** elements, the src attribute can be a relative URL or an absolute URL. Without a src attribute, an img element has no image to load.

***So for example, if your image is called dinosaur.jpg, and it sits in the same directory as your HTML page, you could embed the image like so:***

- < img src="dinosaur.jpg" alt="Dinosaur" />
Copy to Clipboard
If the image was in an images subdirectory, which was inside the same directory as the HTML page, then you'd embed it like this:

- < img src="images/dinosaur.jpg" alt="Dinosaur" />


**Note:** Search engines also read image filenames and count them towards SEO. Therefore, you should give your image a descriptive filename; dinosaur.jpg is better than img835.png.

***You could embed the image using its absolute URL, for example:***

- < img src="https://www.example.com/images/dinosaur.jpg" alt="Dinosaur" />

But this is not recommended. You should host your own images, which in simple setups means keeping the images for your website on the same server as your HTML. In more advanced setups, you might use a CDN (Content Delivery Network) to deliver your images.

**Warning:** Never point your src attribute at an image hosted on someone else's website without permission. This is called "hotlinking". It is generally considered unethical, since someone else would be paying the bandwidth costs for delivering the image when someone visits your page. It also leaves you with no control over whether the image is removed or replaced with something embarrassing.

In general, you should host the images you want to use on your site. Keep in mind that many images you may find on the web are copyrighted. Before you host an image, you should make sure that one of these applies:

- You own the image.

- You have received explicit, written permission from the image owner.

- You have ample proof that the image is, in fact, in the public domain.

**Note:** Elements like **< img>** and **< video>** are sometimes referred to as replaced elements. This is because the element's content and size are defined by an external resource (like an image or video file), not by the contents of the element itself. You can read more about them at Replaced elements.

Alternative text
The next attribute we'll look at is alt. Its value is supposed to be a textual description of the image, for use in situations where the image cannot be seen/displayed or takes a long time to render because of a slow internet connection. For example, our above code could be modified like so:

<img
  src="images/dinosaur.jpg"
  alt="The head and torso of a dinosaur skeleton;
          it has a large head with long sharp teeth" />
Copy to Clipboard
The easiest way to test your alt text is to purposely misspell your filename. If for example our image name was spelled dinosooooor.jpg, the browser wouldn't display the image, and would display the alt text instead

So, why would you ever see or need alt text? It can come in handy for a number of reasons:

The user is visually impaired, and is using a screen reader to read the web out to them. In fact, having alt text available to describe images is useful to most users.
As described above, the spelling of the file or path name might be wrong.
The browser doesn't support the image type. Some people still use text-only browsers, such as Lynx, which displays the alt text of images.
You may want to provide text for search engines to utilize; for example, search engines can match alt text with search queries.
Users have turned off images to reduce data transfer volume and distractions. This is especially common on mobile phones, and in countries where bandwidth is limited or expensive.
What exactly should you write inside your alt attribute? It depends on why the image is there in the first place. In other words, what you lose if your image doesn't show up:

Decoration. You should use CSS background images for decorative images, but if you must use HTML, add a blank alt="". If the image isn't part of the content, a screen reader shouldn't waste time reading it.
Content. If your image provides significant information, provide the same information in a brief alt text – or even better, in the main text which everybody can see. Don't write redundant alt text. How annoying would it be for a sighted user if all paragraphs were written twice in the main content? If the image is described adequately by the main text body, you can just use alt="".
Link. If you put an image inside <a> tags, to turn an image into a link, you still must provide accessible link text. In such cases you may, either, write it inside the same <a> element, or inside the image's alt attribute – whichever works best in your case.
Text. You should not put your text into images. If your main heading needs a drop shadow, for example, use CSS for that rather than putting the text into an image. However, If you really can't avoid doing this, you should supply the text inside the alt attribute.
Essentially, the key is to deliver a usable experience, even when the images can't be seen. This ensures all users are not missing any of the content. Try turning off images in your browser and see how things look. You'll soon realize how helpful alt text is if the image cannot be seen.

Note: For more information, see our guide to Text Alternatives.

Width and height
You can use the width and height attributes to specify the width and height of your image. You can find your image's width and height in a number of ways. For example on the Mac you can use Cmd + I to get the info display up for the image file. 

However, you shouldn't alter the size of your images using HTML attributes. If you set the image size too big, you'll end up with images that look grainy, fuzzy, or too small, and wasting bandwidth downloading an image that is not fitting the user's needs. The image may also end up looking distorted, if you don't maintain the correct aspect ratio. You should use an image editor to put your image at the correct size before putting it on your webpage.

Note: If you do need to alter an image's size, you should use CSS instead.

Image titles
As with links, you can also add title attributes to images, to provide further supporting information if needed.

However, this is not recommended — title has a number of accessibility problems, mainly based around the fact that screen reader support is very unpredictable and most browsers won't show it unless you are hovering with a mouse (so e.g. no access to keyboard users).

-----

Images, Color, Text, and More Work with Functions
HTML Media Q&A
What is a real world use case for the alt attribute being used in a website?

If an image doesn’t load in a website, the alt tag will pull up what the image would’ve been.
How can you improve accessibility of images in an HTML document?

The way you improve accessbility of images in HTML documents is by adding an alt tag and filing it out with the information in case an element doesn’t load or someone is using a screen reader.
Provide an example of when the figure element would be useful in an HTML document.

An example of when the figure element would be useful is if you’re adding an image or video that incldues a description with it.
Describe the difference between a gif image and an svg image, pretend you are explaining to an elder in your community.

Gif images are larger than SVG and have more complicated and longer animations. The file size of a gif is much larger than a SVG.
SVG images are more ideal for high quality images and can be scale to ANY size. The file size of a svg is much smaller than a GIF.
What image type would you use to display a screenshot on your website and why?

The image type I would display a screenshot with on my website would be .png due the clear image quality
Learn CSS Q&A
Describe the difference between foreground and background colors of an HTML element, pretend you are talking to someone with no technical knowledge.

Color defines the foreground. This is the text on the overall webpage(s).
Background-color defines the background. This is the color on the webpage(s).
Your friend asks you to give his colorless blog website a touch up. How would you use color to give his blog some character?

I would use a background tag to color his background. I’d also attach the color tag to the font to change the colors or the divs to give the backing of the words color block. All images and videos would also have a color boarder.
What should you consider when choosing fonts for an HTML document?

If they have bold and italtics in their font-style
Readability
Functionality
Translating to other langauges
What do font-size, font-weight, and font-style do to HTML text elements?

Font-Size: this changes the size of the font
Font-Weight: this changes the line thickness of the font
Font-Style: this changes the font-type such as if you want it to be strong, bold, or italic
Describe two ways you could add spacing around the characters displayed in an h1 element.

You can use the word-spacing or letter-spacing element to adjust the spacing of an h1 element
Word-Spacing: spaces the words in the text element to the determined width
Text-Spacing: spaces the letters in each word in a text element to the deteremined width
Examples:

p::first-line {
  letter-spacing: 4px;
  word-spacing: 4px;
}
Things I want to know more about
I want to know if you can add custom fonts to websites

I want to know if I can set the background image to a certain side for all devices

I want to know if I can have several different colors to a background without having use an image.

I want to know if I can add gradience to a background.

Websites for Reference
HTML
https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding

https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Images_in_HTML

https://developer.mozilla.org/en-US/docs/Web/Media/Formats/Image_types#choosing_an_image_format

CSS
https://developer.mozilla.org/en-US/docs/Learn/CSS

https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Colors/Applying_color

https://developer.mozilla.org/en-US/docs/Learn/CSS/Styling_text/Fundamentals