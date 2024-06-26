# HTML

### Hypertext:

text (often with embeds such as images, too) that is organized in order to connect related items

### Markup:

a style guide for typesetting anything to be printed in hardcopy or soft copy format

### Language:

a language that a computer system understands and uses to interpret commands.

HTML determines the structure of web pages. This structure alone is not enough to make a web page look good and interactive. So you'll use assisted technologies such as CSS and JavaScript to make your HTML beautiful and add interactivity, respectively.

## <!DOCTYPE>

The `<!DOCTYPE>` declaration represents the document type, and helps browsers to display web pages correctly.

It must only appear once, at the top of the page (before any HTML tags).

The `<!DOCTYPE>` declaration is not case sensitive.

## Semantic HTML

Semantic HTML means that your HTML tags convey the actual meaning of what they are used for.

- `<header>`: The `<header>` element defines the introductory section of a web page. It contains items such as the logo, navigation, theme switcher, and search bar.

- `<nav>`: The `<nav>` element specifies the navigation items of the page such as home, contact, about, FAQs, and so on.

- `<main>`: The `<main>` element is conventionally treated as the immediate descendant of the tag. It contains the main sections of the HTML document apart from `<header>` and `<footer>`. Ideally, there should be just one of these in the whole HTML document.

- `<section>`: The `<section>` element defines a particular section of the web page. This may be the showcase section, about section, contact section, or others. You can use numerous sections in a single HTML document.

- `<article>`: The `<article>` element represents a certain part of a web page that conveys some particular information. Such information could be a combination of text, images, videos, and embeds. Look at this element as a standalone blog post on a page containing excerpts about other blog posts.

- `<aside>`: As the name implies, this represents a sidebar on a web page. It is usually a part of the web page that is not directly related to the main content.

- `<footer>`: The `<footer>` element accommodates items such as quick links, copyright information, or any other data related to the entire website or web page.

## Header Tags

```html
<h1></h1>
<h2></h2>
<h3></h3>
<h4></h4>
<h5></h5>
<h6></h6>
```

## Paragraph Tags

```html
<p>This is a paragraph.</p>
<p>This is another paragraph.</p>
```

## Links

HTML links are defined with the <a> tag:

```html
<a href="https://www.github.com">This is a link</a>
```

## Images

HTML images are defined with the `<img>` tag.

The source file (src), alternative text (alt), width, and height are provided as attributes:

```html
<img src="pfp.jpg" alt="Picture of Me" width="104" height="142" />
```

## HTML Entities

- `&nbsp;`: Non breaking space
- `&lt;`:< less than
- `&gt;`: > greater than
- `&amp;`: ampersand
- `&quot;`: Double Quotation
- `&apos;`: Single Quotation
- `&cent;`: cent
- `&pound;`: pound
- `&yen;`: yen
- `&euro;`: euro
- `&copy;`: copyright
- `&reg;`: trademark

## Nested Elements

HTML elements can be nested (this means that elements can contain other elements).

All HTML documents consist of nested HTML elements.

The following example contains four HTML elements (`<html>`, `<body>`, `<h1>` and `<p>`)

```html
<!DOCTYPE html>
<html>
  <body>
    <h1>My First Heading</h1>
    <p>My first paragraph.</p>
  </body>
</html>
```

## Ordered List

An ordered list starts with the `<ol>` tag. Each list item starts with the `<li>` tag.

```html
<ol>
  <li>Item#1</li>
  <li>Item#2</li>
  <li>Item#3</li>
</ol>
```

## Unordered list

An unordered list starts with the `<ul>` tag. Each list item starts with the `<li>` tag.

```html
<ul>
  <li>Item#1</li>
  <li>Item#2</li>
  <li>Item#3</li>
</ul>
```

## Description Lists

The `<dl>` tag defines the description list, the `<dt>` tag defines the term (name), and the `<dd>` tag describes each term:

```html
<dl>
  <dt>Item#1</dt>
  <dd>- description</dd>
  <dt>Item#2</dt>
  <dd>- description</dd>
</dl>
```

## Forms

The HTML `<form>` element is used to create an HTML form for user input

### Input Fields

The HTML `<input>` element is the most used form element.

An `<input>` element can be displayed in many ways, depending on the type attribute.

- `<input type="text">` Displays a single-line text input field
- `<input type="radio">` Displays a radio button (for selecting one of many choices)
- `<input type="checkbox">` Displays a checkbox (for selecting zero or more of many choices)
- `<input type="submit">` Displays a submit button (for submitting the form)
- `<input type="button">` Displays a clickable button

### Text Fields

The `<input type="text">` defines a single-line input field for text input.

The `<label>` tag defines a label for many form elements.

The `<label>` element is useful for screen-reader users, because the screen-reader will read out loud the label when the user focuses on the input element.

```html
<form>
  <label for="fname">First name:</label><br />
  <input type="text" id="fname" name="fname" /><br />
  <label for="lname">Last name:</label><br />
  <input type="text" id="lname" name="lname" />
</form>
```

### Select

The `<select>` element defines a drop-down list:

```html
<label for="cars">Choose a car:</label>
<select id="cars" name="cars">
  <option value="volvo">Volvo</option>
  <option value="saab">Saab</option>
  <option value="fiat">Fiat</option>
  <option value="audi">Audi</option>
</select>
```

The `<option>` element defines an option that can be selected.

To define a pre-selected option, add the `selected` attribute to the option

### Button Element

The `<button>` element defines a clickable button:

```html
<button type="button" onclick="alert('Hello World!')">Click Me!</button>
```

### The `<fieldset>` and `<legend>` Elements

The `<fieldset>` element is used to group related data in a form.

The `<legend>` element defines a caption for the `<fieldset>` element.

```html
<form action="/action_page.php">
  <fieldset>
    <legend>Personalia:</legend>
    <label for="fname">First name:</label><br />
    <input type="text" id="fname" name="fname" value="John" /><br />
    <label for="lname">Last name:</label><br />
    <input type="text" id="lname" name="lname" value="Doe" /><br /><br />
    <input type="submit" value="Submit" />
  </fieldset>
</form>
```

## Tables

Example:

```html
<table>
  <tr>
    <th>Company</th>
    <th>Contact</th>
    <th>Country</th>
  </tr>
  <tr>
    <td>Alfreds Futterkiste</td>
    <td>Maria Anders</td>
    <td>Germany</td>
  </tr>
  <tr>
    <td>Centro comercial Moctezuma</td>
    <td>Francisco Chang</td>
    <td>Mexico</td>
  </tr>
</table>
```

### Table Cells

Each table cell is defined by a `<td>` and a `</td>` tag.

td stands for table data.

Everything between `<td>` and `</td>` are the content of the table cell.

```html
<table>
  <tr>
    <td>Emil</td>
    <td>Tobias</td>
    <td>Linus</td>
  </tr>
</table>
```

## Empty Elements

- `<br>`: Line break
- `<strong>`: Defines important text, typically displayed in bold.
- `<i>`: Defines italic text.
- `<em>`: Defines emphasized text, typically displayed in italics.
- `<u>`: tag is used to underline text in HTML
- `<hr>`: element is used to separate content (or define a change) in an HTML page
- `<sub>`: Defines subscript text, which appears below the baseline of the text.
- `<sup>`: Defines superscript text, which appears above the baseline of the text.
- `<del>`:indicate deleted or removed text
- `<pre>`:Defines pre-formatted text
- `<mark>`: Marked text
- `<small>`: Smaller text
- `<ins>`: Inserted text
- `<img>`: Image
- `<input>`: Input field
- `<hr>`: Horizontal rule
- `<meta>`: Metadata
- `<link>`: Link reference
- `<area>`: Defines an area inside an image map
- `<base>`: Defines a base URL for all relative URLs in a document
- `<col>`: Defines column properties for each column within a `<colgroup>` element
- `<embed>`: Embeds external content
- `<keygen>`: Generates a key pair for forms
- `<param>`: Defines parameters for objects
- `<source>`: Defines multiple media resources for media elements like `<video>` and `<audio>`
- `<track>`: Defines text tracks for media elements
- `<wbr>`: Word break opportunity

## Quotation and Citation Elements

- `<blockquote>`: Used to indicate that a block of text is a quotation from another source. It typically renders as indented text.
- `<q>`: Stands for "inline quotation". It's used for short inline quotations. Browsers usually render the content inside `<q>` with quotation marks.
- `<abbr>`: Stands for "abbreviation". It's used to mark up abbreviations or acronyms in a document. You can include the full form of the abbreviation using the title attribute.
- `<address>`: Indicates contact information for the author of a document or an article. It's typically used to include contact details like an email address, physical address, or phone number.
- `<cite>`: Used to mark up the title of a work, such as a book, movie, or paper. It's often used in combination with other elements like `<blockquote>` or `<q>` to provide the citation for a quotation.
- `<bdo>`: Stands for "bi-directional override". It's used to override the default text directionality of the content. This can be useful when you need to display text in a different direction, such as from right-to-left instead of left-to-right.

## Block-level Elements

- `<address>`
- `<article>`
- `<aside>`
- `<blockquote>`
- `<canvas>`
- `<dd>`
- `<div>`
- `<dl>`
- `<dt>`
- `<fieldset>`
- `<figcaption>`
- `<figure>`
- `<footer>`
- `<form>`
- `<h1>-<h6>`
- `<header>`
- `<hr>`
- `<li>`
- `<main>`
- `<nav>`
- `<noscript>`
- `<ol>`
- `<p>`
- `<pre>`
- `<section>`
- `<table>`
- `<tfoot>`
- `<ul>`
- `<video>`

## Inline Elements

- `<a>`
- `<abbr>`
- `<acronym>`
- `<b>`
- `<bdo>`
- `<big>`
- `<br>`
- `<button>`
- `<cite>`
- `<code>`
- `<dfn>`
- `<em>`
- `<i>`
- `<img>`
- `<input>`
- `<kbd>`
- `<label>`
- `<map>`
- `<object>`
- `<output>`
- `<q>`
- `<samp>`
- `<script>`
- `<select>`
- `<small>`
- `<span>`
- `<strong>`
- `<sub>`
- `<sup>`
- `<textarea>`
- `<time>`
- `<tt>`
- `<var>`
