# How the Web Works

## What is the internet, actually?
[![Diagram depicting servers, clients and ISP](http://img.youtube.com/vi/7_LPdttKXPc/0.jpg)](http://www.youtube.com/watch?v=7_LPdttKXPc)

## What is a web page?

## What is HTML?

- Hyper Text Markup Language
- Content
- Tag
- Element
- Attribute


## How do you make a web page?

You need:
- A [text editor](https://www.sublimetext.com/)
- A folder for your web page
- An index.html file
- A browser

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

### Try it out

Add an image tag to index.hmtl that tells the browser where to find the image.

### How's it look?

![gif of a Star Wars robot giving a lighter thumbs-up](https://media.giphy.com/media/3o7abB06u9bNzA8lu8/giphy.gif)

### Getting fancier

- Add an "alt" attribute to your `<img>` tag so that people using screen readers will know what's in the image.
- Change the size of your image using the "height" and "width" attributes.

## How do you make your web page look even more exciting?

Add CSS to modify the presentation of the elements. Remeber, HTML specifies what kind of thing a piece of content is, and CSS controls how that piece of content appears to the user.

## What is CSS?

CSS stands for Cascading Style Sheet. The "Style Sheet" part means that the document tells your website how to style all the different components. The "Cascading" part means that CSS operates according to a hierarchy of specificity. The more specific rule always wins. For example:

```
.p {
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

You need:
- A styles.css file
- A way to tell your web page where to find the styles.css file

## Try it out

1. Create a file called styles.css.
2. Edit your index.html file to tell it where to find styles.css.
3. Create a class in your stylesheet with a unique name.
4. Define the class so that it changes the color and the size of text.
5. Assign the class to a `<p>` element in your website.

### How's it look?
![gif of Jessica Williams looking excited](https://media.giphy.com/media/3o7abBP0nMjrdIvaCY/giphy.gif)

## Testing out CSS hierarchies
1. Create a class that adds a strikethrough through all `<h3>` elements.
2. Create a second class called "rightside" that aligns anything in the class to the right.
3. Add three elements to your website:
- Something with an `<h3>` tag
- Something with the class "rightside"
- Something with both an `<h3>` tag and the class "rightside"
4. Open the page in your browser and compare.
