# HTML structure

Category: Fundamentals of HTML

HTML files require certain elements to set up the document properly. We can let web browsers know that we are using HTML by starting our document with a *document type declaration*.

The declaration looks like this:

```html
<!DOCTYPE html>
```

This declaration is an instruction, and it must be the first line of code in your HTML document. It tells the browser what type of document to expect, along with what version of HTML is being used in the document.

To create HTML structure and content, we must add opening and closing [`<html>`](https://www.codecademy.com/resources/docs/html/elements/html?page_ref=catalog) tags after declaring `<!DOCTYPE html>`:

```html
<!DOCTYPE html>
<html>

</html>
```

Head:

The `<head>`element is part of this HTML metaphor. It goes above our `<body>` element.

The `<head>` element contains the *metadata* for a web page. Metadata is information about the page that isn’t displayed directly on the web page. Unlike the information inside of the `<body>` tag, the metadata in the head is information about the page itself.

A browser’s tab displays the title specified in the [`<title>`](https://www.codecademy.com/resources/docs/html/attributes/title?page_ref=catalog) tag. The `<title>` tag is always inside of the `<head>`.

Links:

You can add [links](https://www.codecademy.com/resources/docs/html/links) to a web page by adding an *anchor* element [`<a>`](https://www.codecademy.com/resources/docs/html/elements/a?page_ref=catalog) and including the text of the link in between the opening and closing [tags](https://www.codecademy.com/resources/docs/html/tags).

```html
<a href="https://www.wikipedia.org/">This Is A Link To Wikipedia</a>
```

The `target` attribute specifies how a link should open.

It’s possible that one or more links on your web page link to an entirely different website. In that case, you may want users to read the linked website, but hope that they return to your web page. This is exactly when the `target` attribute is useful!

```html
<a href="https://en.wikipedia.org/wiki/Brown_bear" target="_blank">The Brown Bear</a>
```

Linking to Relative Page:

HTML files are often stored in the same folder, as shown in the example above. If the browser is currently displaying **index.html**, it also knows that **about.html** and **contact.html** are in the same folder. Because the files are stored in the same folder, we can link web pages together using a *relative path*.

```html
<a href="./contact.html">Contact</a>
```

A relative path is a filename that shows the path to a *local file* (a file on the same website, such as `./index.html`) versus an absolute path (a full URL, like `https://www.codecademy.com/learn/learn-html` which is stored in a different folder). The `./` in `./index.html` tells the browser to look for the file in the current folder.

Linking at will: (on image, some other content)

HTML allows you to turn nearly any element into a link by wrapping that element with an anchor element. With this technique, it’s possible to turn images into links by simply wrapping the [`<img>`](https://www.codecademy.com/resources/docs/html/elements/img?page_ref=catalog) element with an `<a>` element.

```html
<a href="https://en.wikipedia.org/wiki/Opuntia" target="_blank">
	<img src="https://www.Prickly_Pear_Closeup.jpg" alt="A red prickly pear fruit"/></a>
```

Linking to same page:

When users visit our site, we want them to be able to click a link and have the page automatically scroll to a specific section.

In order to link to a target on the same page, we must give the target an `id` attribute and a unique value like this:

```html
<p id="top">This is the top of the page!</p>
<h1 id="bottom">This is the bottom! </h1>
```

An `id` should be descriptive to make it easier to remember the purpose of a link. The target link is a string containing the `#` character and the target element’s `id`.

Comments:

HTML files also allow you to add [comments](https://www.codecademy.com/resources/docs/html/comments?page_ref=catalog) to your code.

Comments begin with `<!--` and end with `-->`. Any characters in between will be ignored by your browser.

```html
<!-- This is a comment that the browser will not display. -->
```