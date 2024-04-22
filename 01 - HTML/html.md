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

## Empty Elements

`<br>: Line break`
`<strong>: Defines important text, typically displayed in bold.`
`<i>: Defines italic text.`
`<em>: Defines emphasized text, typically displayed in italics.`
`<u> tag is used to underline text in HTML`
`<hr>: element is used to separate content (or define a change) in an HTML page`
`<sub>: Defines subscript text, which appears below the baseline of the text.`
`<sup>: Defines superscript text, which appears above the baseline of the text.`
`<del>:indicate deleted or removed text`
`<pre>:Defines pre-formatted text`
`<mark> - Marked text`
`<small> - Smaller text`
`<ins> - Inserted text`
`<img>: Image`
`<input>: Input field`
`<hr>: Horizontal rule`
`<meta>: Metadata`
`<link>: Link reference`
`<area>: Defines an area inside an image map`
`<base>: Defines a base URL for all relative URLs in a document`
`<col>: Defines column properties for each column within a <colgroup> element`
`<embed>: Embeds external content`
`<keygen>: Generates a key pair for forms`
`<param>: Defines parameters for objects`
`<source>: Defines multiple media resources for media elements like <video> and <audio>`
`<track>: Defines text tracks for media elements`
`<wbr>: Word break opportunity`

## Quotation and Citation Elements

`<blockquote>`: Used to indicate that a block of text is a quotation from another source. It typically renders as indented text.
<q>: Stands for "inline quotation". It's used for short inline quotations. Browsers usually render the content inside <q> with quotation marks.
<abbr>: Stands for "abbreviation". It's used to mark up abbreviations or acronyms in a document. You can include the full form of the abbreviation using the title attribute.

<address>: Indicates contact information for the author of a document or an article. It's typically used to include contact details like an email address, physical address, or phone number.
<cite>: Used to mark up the title of a work, such as a book, movie, or paper. It's often used in combination with other elements like <blockquote> or <q> to provide the citation for a quotation.
<bdo>: Stands for "bi-directional override". It's used to override the default text directionality of the content. This can be useful when you need to display text in a different direction, such as from right-to-left instead of left-to-right.
