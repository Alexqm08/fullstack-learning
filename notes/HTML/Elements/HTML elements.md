# HTML elements

Category: Fundamentals of HTML
Summary: HTML is structured with elements such as `<body>`, headings, `<div>`, and lists. Attributes like id enhance elements, while tags like `<img>` and `<video>` allow media integration. Proper use of `<alt>` text improves accessibility and SEO.

<aside>
🔗

https://www.codecademy.com/resources/docs/html

https://www.codecademy.com/workspaces/new

https://www.youtube.com/watch?v=uxmB8MlO3m8&t=691s

</aside>

HTML structure:

HTML is organized as a collection of family tree relationships. As you saw in the last exercise, we placed `<p>` tags within `<body>` tags. When an element is contained inside another element, it is considered the *child* of that element. The child element is said to be *nested* inside of the *parent* element.

```html
<body>
<p>This paragraph is a child of the body</p>
</body>
```

The body:
One of the key HTML [elements](https://www.codecademy.com/resources/docs/html/elements) we use to build a webpage is the *body* element. Only content inside the opening and closing body [tags](https://www.codecademy.com/resources/docs/html/tags) can be displayed to the screen.

`<body>  </body>`

Headings:

Headings in HTML are similar to headings in other types of media.

```html
<body>
  <h1>The Brown Bear</h1>
  <h2>About Brown Bears</h2>
  <h3>Species</h3>
  <h3>Features</h3>
  ...
  <h6>Functionc</h6>
</body>
```

the smallest one is h6.

Divs:

[`<div>`](https://www.codecademy.com/resources/docs/html/elements/div?page_ref=catalog) is short for “division” or a container that divides the page into sections. These sections are very useful for grouping elements in your HTML together.

```html
<body>
  <div>
    <h1>Why use divs?</h1>
    <p>Great for grouping elements!</p>
  </div>
</body>
```

`<div>`s allow us to group HTML elements to apply the same styles for all HTML elements inside

Attributes:

[Attributes](https://www.codecademy.com/resources/docs/html/attributes?page_ref=catalog) are content added to the opening tag of an element and can be used in several different ways, from providing information to changing styling. Attributes are made up of the following two parts:

- The *name* of the attribute
- The *value* of the attribute

One commonly used attribute is the `id`. We can use the `id` attribute to specify different content (such as `<div>`s) and is really helpful when you use an element more than once

```html
<div id="intro">
  <h1>Introduction</h1>
</div>
```

Displaying text:

If you want to display text in HTML, you can use a *paragraph* or *span*:

- [*Paragraphs* (`<p>`)](https://www.codecademy.com/resources/docs/html/elements/p) contain a block of plain text.
- [`<span>`](https://www.codecademy.com/resources/docs/html/elements/span?page_ref=catalog) contains short pieces of text or other HTML. They are used to separate small pieces of content that are on the same line as other content.

```html
<div>
  <h1>Technology</h1>
</div>
<div>
  <p><span>Self-driving cars</span> are anticipated to replace up to 2 million jobs over the next two decades.</p>
</div>
```

Styling text:

- The `<em>` tag will generally render as *italic* emphasis.
- The `<strong>` will generally render as **bold** emphasis.

Line breaks:

If you are interested in modifying the spacing in the browser, you can use HTML’s *line break* element: `<br>`. The line break element is unique because it is only composed of a starting tag. You can use it anywhere within your HTML code and a line break will be shown in the browser.

```html
<p>The Nile River is the longest river <br> in the world, measuring over 6,850 <br> kilometers long (approximately 4,260 <br> miles).</p>
```

Unordered list:

In HTML, you can use an *unordered list* tag (`<ul>`) to create a list of items in no particular order. An unordered list outlines individual *list items* with a bullet point.

The `<li>` or list item tag is used to describe an item in a list.

```html
<ul>
  <li>Limes</li>
  <li>Tortillas</li>
  <li>Chicken</li>
</ul>
```

Ordered list:

[*Ordered lists* (`<ol>`)](https://www.codecademy.com/resources/docs/html/elements/ol?page_ref=catalog) are like unordered lists, except that each list item is numbered. They are useful when you need to list different steps in a process or rank items for first to last.

You can create the ordered list with the `<ol>` tag and then add individual list items to the list using `<li>` tags.

```html
<ol>
  <li>Preheat the oven to 350 degrees.</li>
  <li>Mix whole wheat flour, baking soda, and salt.</li>
  <li>Cream the butter, sugar in separate bowl.</li>
  <li>Add eggs and vanilla extract to bowl.</li>
</ol>
```

Image:

The `<img>` tag allows you to add an image to a web page. Most elements require both opening and closing tags, but the `<img>` tag is a *self-closing tag*. Note that the end of the `<img>` tag has a forward slash `/`.

```html
<img src="image-location.jpg" />
```

The `<img>` tag has a required *attribute* called `src`. The `src` attribute must be set to the image’s *source*, or the location of the image.

Image alts:

The `alt` attribute, which means alternative text, brings meaning to the [images](https://www.codecademy.com/resources/docs/html/images) on our sites. The `alt` attribute can be added to the image tag just like the [`src`](https://www.codecademy.com/resources/docs/html/attributes/src) attribute. The value of `alt` should be a description of the image.

```html
<img src="#" alt="A field of yellow sunflowers" />
```

The `alt` attribute also serves the following purposes:

- If an image fails to load on a web page, a user can mouse over the area originally intended for the image and read a brief description of the image. This is made possible by the description you provide in the `alt` attribute.
- Visually impaired users often browse the web with the aid of screen reading software. When you include the `alt` attribute, the screen reading software can read the image’s description out loud to the visually impaired user.
- The `alt` attribute also plays a role in Search Engine Optimization (SEO), because search engines cannot “see” the images on websites as they crawl the internet. Having descriptive `alt` [attributes](https://www.codecademy.com/resources/docs/html/attributes) can improve the ranking of your site.

Videos:

Like the `<img>` element, the `<video>` element requires a `src` attribute with a link to the video source. Unlike the `<img>` element however, the `<video>` element requires an opening and a closing tag.

```html
<video src="myVideo.mp4" width="320" height="240" controls>
  Video not supported
</video>
```