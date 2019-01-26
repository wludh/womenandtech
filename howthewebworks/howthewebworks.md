# How the Web Works

## What is the internet, actually?
[![Diagram depicting servers, clients and ISP](http://img.youtube.com/vi/7_LPdttKXPc/0.jpg)](http://www.youtube.com/watch?v=7_LPdttKXPc)

## What is a web page?

A web page is a document that can be displayed in a browser. A collection of web pages that is grouped together and connected is generally called a website. Web pages can involve a number of different programming languages, but the building block of all web pages is HTML.

## What is HTML?

[This page](https://www.w3schools.com/html/html_intro.asp) has a pretty good description, including this list:
- HTML stands for Hyper Text Markup Language
- HTML describes the structure of web pages using markup
- HTML elements are the building blocks of HTML pages
- HTML elements are represented by tags
- HTML tags label pieces of content such as "heading", "paragraph", "table", and so on
- Browsers do not display the HTML tags, but use them to render the content of the page

### Tags

HTML tags are element names surrounded by angle brackets. Most tags come in pairs, with the starting tag coming right before the content that it marks, and the ending tag coming right after. The end tag looks just like the start tag, but with a forward slash right before the tag name.

For example:

```
<h3>The H3 tags tell the browser that the content between the tags constitutes a subheading</h3>

<p>The paragraph tags tell the browser that the content between the tags constitutes a paragraph.</p>

<i>The i tags tell the browser that the content between the tags should be in italics</i>
```

What's that actually look like?

<h3>The H3 tags tell the browser that the content between the tags constitutes a subheading</h3>

<p>The paragraph tags tell the browser that the content between the tags constitutes a paragraph.</p>

*The i tags tell the browser that the content between the tags should be in italics*

## How do you make a web page?

You need:
- A [text editor](https://www.sublimetext.com/)
- A folder for your web page
- An index.html file
- A browser

### What goes in your HTML document?

Anything you want, really, but you will need a few specific things:
- Your document should start with a document type declaration: `<!DOCTYPE html>`
- The document itself begins with `<html>` and ends with `</html>`
- The part of the document that a browser makes visible goes between `<body>` and `</body>`
- Before the `<body>` section, it's helpful to include some information about the page between `<head>` and `</head>`
- Information in the `<head>` section includes a link to a stylesheet (more on this later), the title of your site between `<title>` and `</title>`, and [other metadata](https://www.w3schools.com/html/html_head.asp)

## Try it out

1. Create a folder on your desktop called "website."
2. Inside the folder, create a file called index.html.
3. Using a text editor, add the following text to index.html:
```
<!DOCTYPE html>

<html>
<head>
	<title>Your website title goes here</title>
</head>

<body>
</body>
</html>
```

4. Add some text in between the `<body>` tags.
5. Open your website using a browser.

### How's it look?

![gif of Michelle Tanner looking disappointed](https://media.giphy.com/media/MC8hMWWQ8wgtW/giphy.gif)

## How do you make your web page look more exciting?

Well, you add more content, for one thing. You can also tag that content using HTML to tell the browser what kind of thing each piece of text is.

### Elements

An HTML element is everything from the start tag to the end tag. This is a `<p>` element:

`<p>The paragraph tags tell the browser that the content between the tags constitutes a paragraph.</p>`

But elements can also be nested. That is, you can have an element inside another element. For instance:

```
<body>
	<h3>The H3 tags tell the browser that the content between the tags constitutes a subheading</h3>
	<i>The i tags tell the browser that the content between the tags should be in italics</i>
</body>
```

The `<h3>` and `<i>` elements are part of the content of the `<body>` element. 

### Attributes

All HTML elements can have attributes, though they don't all have to. Attributes provide additional information about an element, and usually come in name/value pairs like: name="value".

The kind of attributes an element can have is defined by the start tag--different tags have different elements. For example, HTML links are defined by the `<a>` tag. So, a link in HTML might look like this:

`<a>Here's a description of the link</a>`

See any problems with that element?

![cartoon of Wile E. Coyote running into a tunnel painted onto a wall](https://thumbs.gfycat.com/OrderlyIncompleteHoki-small.gif)

It doesn't tell you where the link goes, meaning it doesn't actually go anywhere.

The `<a>` element needs an attribute that gives the URL for the link. In this case, the name of the attribute is "src," and the value is the URL that the link should direct to.

`<a src="http://www.wlu.edu">Here's a description of the link</a>`

## Try it out

Add some more content and some tags to go along:
- At least two [headings](https://www.w3schools.com/html/html_headings.asp) (but only one h1 tag)
- A [list](https://www.w3schools.com/html/html_lists.asp)
- A [link](https://www.w3schools.com/html/html_links.asp)
- A [comment](https://www.w3schools.com/html/html_comments.asp)
- A [blockquote](https://www.w3schools.com/html/html_quotation_elements.asp)

### How's it look?

![gif of Cher from Clueless looking uncertain](https://media.giphy.com/media/yj5oYHjoIwv28/giphy.gif)

## My website needs pictures

Of course it does! But where do you get the pictures? And where do they go?

### File structures

![diagram of folders and subfolders](https://zapier.cachefly.net/storage/photos/afcb5e29842a4dde75d47627f506941a.png)

(There are no diagrams of file structures that aren't boring)

- Create a folder for your images
- Find an image and save it to your images folder

### Image tags
You website needs to tell the browser where to find your image, and how to display it. At a bare minimum, you need to include the path to your image in an `<img>` tag:

`<img src="pathtoimage">`

Quick terminology review: "src" is an attribute of the element "img"

### Try it out

Add an image tag to index.hmtl that tells the browser where to find the image.

### How's it look?

![gif of a Star Wars robot giving a lighter thumbs-up](https://media.giphy.com/media/3o7abB06u9bNzA8lu8/giphy.gif)

### Getting fancier

- Add an "alt" attribute to your `<img>` tag so that people using screen readers will know what's in the image.
- Change the size of your image using the "height" and "width" attributes.

## What if I want more than one page?
Sure, single page websites are cool, but you might need a second page for all your awesome content. To create a second page, start a new text document and save it with a meaningful name and the .html extension. Maybe `about.html`? Your new document should live in the same folder with `index.html`. To link to your second page, add a link on your first and give the name of the file in the href. 

```
<a href="about.html">About page</a>
```
Remember, file structure matters. If you have a complex site with lots of files and folders, you'll need to include them in your link path. How many folders are there in this link? 

```http://www.wlu.edu/the-williams-school/departments-and-programs/accounting```

## How do you make your web page look even more exciting?

Add CSS to modify the presentation of the elements. Remeber, HTML specifies what kind of thing a piece of content is, and CSS controls how that piece of content appears to the user.

## What is CSS?

CSS stands for Cascading Style Sheet. The "Style Sheet" part means that the document tells your website how to style all the different components. The "Cascading" part means that CSS operates according to a hierarchy of specificity. The more specific rule always wins. For example:

```
p {
	font-style: italic;
}

.morespecific {
	color: purple;
}
``` 

`<p>Here's a paragraph</p>` will render as follows:

![A line of blue text that reads "Here's a paragraph"](./blue.png)

But `<p class="morespecific">Here's a more specific paragraph</p>` will render in this way:

![A line of purple text that reads "Here's a more specific paragraph"](./purple.png)

## CSS Syntax
With CSS comes a new syntax. First, you state which HTML element (or class/id) you wish to modify (also called a selector). Next, you declare the modifications you want to make in between two curly brackets. The modifications are drawn from a list of CSS properties. It's best to check the documentation so you know, for instance, that "color" means font color and "background-color" means the background of the page. Each of the declarations is another form of a name value pair, except this time they are separated with a colon and followed by a semi-colon (and usually a line break). 

```
body {
	background-color:blue;
	font-family: Arial;
	}
```

## Classes and IDs
CSS makes it easy to be consistent with your styling. But what if you want one paragraph to be blue and another to be green? You can use classes and IDs to distinguish between pieces of content. Classes can be used with multiple elements while IDs should only be used once. In your HTML document, insert the class/id as an attribute of the HTML tag you wish to modify. In your CSS document, you select the class/id using either a `.` or a hash `#`. 

```
<p class="blue">...</p>
<p id="green">...</p>
```

```
.blue {
	color: blue;
}

#green {
	color:green;
}
```


You need:
- A style.css file. Create a new text document in your text editor and save it with the `.css` extension. 
-  A way to tell your web page where to find the style.css file. Insert the following line of code into the `<head>` element in your HTML document: 

```
<link rel="stylesheet" type="text/css" href="style.css">
```

## Try it out

1. Create a file called style.css.
2. Edit your index.html file to tell it where to find style.css.
3. Create a class in your stylesheet with a unique name.
4. Define the class so that it changes the color and the size of text.
5. Assign the class to a `<p>` element in your website.

### How's it look?
![gif of Jessica Williams looking excited](https://media.giphy.com/media/3o7abBP0nMjrdIvaCY/giphy.gif)

## Testing out CSS hierarchies
1. Create a class that [adds a strikethrough](https://www.w3schools.com/cssref/pr_text_text-decoration.asp) to all `<h3>` elements.
2. Create a second class called "rightside" that [aligns anything in the class to the right](https://www.w3schools.com/cssref/pr_text_text-align.asp).
3. Add three elements to your website:
- Something with an `<h3>` tag
- Something with the class "rightside"
- Something with both an `<h3>` tag and the class "rightside"
4. Open the page in your browser and compare.

## Think ahead
When we come back from lunch, we'll start designing your website. Think about what type of website you might want to make. Will be it a portfolio for employers? A gallery of your favorite dog photos? A site for your hobby/nonprofit/business/club? 
