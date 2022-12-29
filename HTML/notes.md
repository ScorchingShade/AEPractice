# HTML - Hypertext markup language

Attributes - attributes are ways to pass extra data to the tags that change the way the browser treats the tags.
This is similar to params being passed to the functions.

e.g. input tag



## HTML
HyperText Markup Language is the primary language of the web, containing the content and structure of a website.

Learn more: https://developer.mozilla.org/en-US/docs/Web/HTML

## Tag
The primary method of marking up content using HTML. Tags use the syntax < tagname>content</ tagname>.

For example, paragraphs use the p tag, so we could create the paragraph "Hello World" with < p>Hello World< /p>.

The left side tag, such as < p>, is referred to as the opening tag. The right side tag, such as </ p> is referred to as the closing tag. Everything inside of the tags is the content, which will actually be rendered on the page. The combination of the opening tag, content and closing tag are referred to as a complete element.

Some tags don't have any content, so we call these empty tags or self-closing tags. These either use the opening tag syntax or < tagname />.

For example, horizontal rules use the hr tag, so we could create a horizontal rule with either < hr> or < hr />.

## Attribute
Extra information provided to HTML elements, similar to function parameters.

Attributes use the syntax < tagname attribute="value">content</ tagname>. The attribute name will always come after the tag name, with a space in between them. The quoted value will then be separated from the attribute name by an equals sign. For example, we can create an input of type "checkbox" with < input type="checkbox" />.

A small number of attributes are booleans rather than strings. Any value for a boolean attribute will be treated as true, so all of the following checkboxes would be disabled.

< input type="checkbox" disabled="disabled" />
< input type="checkbox" disabled="true" />
< input type="checkbox" disabled />

<!--
  This is still disabled, since the attribute is set.
  Of course we don't recommend this though as it is quite confusing to read.
-->
< input type="checkbox" disabled="true" />
<! DOCTYPE html > 
The required first line of every HTML file for telling the browser what version of html to use. A doctype of html will use the modern HTML5 standard. While a page will usually render properly without a doctype declaration, they should still always be included as some older browsers will not render pages following the modern specification without it (this is sometimes called "quirks" mode).

## head tag
The tag containing metadata about the HTML document (i.e. anything that isn't displayed on the page). The < head> of the HTML file should be the first tag within the < html> tag.

The < title> is the only required tag within the < head>. This tag gives the page a title, which is used for the name of the tab in most browsers, and it gets used for search results in many search engines.

Learn more: https://developer.mozilla.org/en-US/docs/Web/HTML/Element/head


## body tag
The tag containing the content of the webpage. The < body> of the HTML file should be the second tag within the  < html> tag, just below the < head>.

Learn more: https://developer.mozilla.org/en-US/docs/Web/HTML/Element/body



## Semantic HTML
HTML that clearly describes the content of the page. HTML loses its semantic meaning when tags are misused, or generic tags (namely <div> and <span>) are overused instead of semantic tags.

Semantic HTML includes the usage of semantic grouping tags, which give meaning to different sections of the page. These are some of the most commonly used semantic grouping tags:

< article>: Self contained, independently distributable content.
< section>: Thematic grouping of content, not self contained.
< header>: Introductory content.
< main>: Main content, limited to one per page.
< nav>: A section of links, oftentimes for the primary navigation of the page.
< aside>: Non-vital content indirectly related to main content. The page would make sense without this content.
< footer>: Footer of the document, oftentimes containing copyright information.




## Key Terms
<hr>
### < p> Tags
The paragraph tag, usually used for blocks of text (although they can contain other elements that are part of the paragraph, such as images). For example:

< p>Hello World!< /p>
Learn more: https://developer.mozilla.org/en-US/docs/Web/HTML/Element/p

<hr>
### Headline Tags
HTML tags represented by < h1> through < h6>. < h1> is the top level heading, while < h2> is a secondary subheading and so on. For example:

< h1>Main Heading</ h1> < h2>Secondary Heading</ h2>
Learn more: https://developer.mozilla.org/en-US/docs/Web/HTML/Element/Heading_Elements
<hr>
### The Img tags
The image tag. This is an empty tag, and it should always include two primary attributes:

src: The path to the image, either relative or absolute.
alt: Alternative text to be used with screen readers or any time the image cannot be displayed.
< img src="img/dog.png" alt="dog" />
Learn more: https://developer.mozilla.org/en-US/docs/Web/HTML/Element/img

<hr>

### ul tag
The unordered list tag, used for a list where the order does not matter. By default, most browsers will show this as a bulleted list.

The unordered list should contain any number of < li> tags. For example:

< ul>
    < li>AlgoExpert</ li>
    < li>SystemsExpert</ li>
    < li>MLExpert</ li>
    < li>FrontendExpert</ li>
</ ul>
Learn more: https://developer.mozilla.org/en-US/docs/Web/HTML/Element/ul

<hr>
### ol tag - ordered list
The ordered list tag, used for a list where the order matters. By default, most browsers will show this as a numbered list.

The ordered list should contain any number of < li> tags. For example:

< ol> < li>Step 1</ li> < li>Step 2</ li> < li>Step 3</ li> </ ol>
Learn more: https://developer.mozilla.org/en-US/docs/Web/HTML/Element/ol

<hr>

### li - list item tags
The list item tag, used for individual elements in both unordered and ordered lists.

List items can also contain other lists to create nested lists. For example:

< ol> < li>Step 1</ li> < li> Step 2: < ol> < li>Substep 1:</ li> < li>Substep 2:</ li> </ ol> </ li> < li>Step 3</ li> </ ol>
Learn more: https://developer.mozilla.org/en-US/docs/Web/HTML/Element/li

<hr>

### pre - preformatted tag
The preformatted text tag. This tag preserves whitespace, which can be useful when indentation and newlines need to be preserved. For example:

<pre>
< pre>
    *
   ***
  *****
 *******
*********
   | |

</pre>

Learn more: https://developer.mozilla.org/en-US/docs/Web/HTML/Element/pre

<hr>

### br - line break
The line break tag. This is an empty tag used to create a line break in text, such as for the introduction of an email or new lines in a poem. However, this tag should not be used just for spacing out elements as that can be accomplished with CSS. For example:

< p> Dear User, < br /> We hope you are enjoying FrontendExpert! </ p>
Learn more: https://developer.mozilla.org/en-US/docs/Web/HTML/Element/br


<hr>

### hr - horizontal rule tag
The horizontal rule tag. This is an empty tag used to create a thematic break between content, drawn as a horizontal line by default. For example:

< p>Part 1</ p> < hr /> < p>Part 2< /p>
Learn more: https://developer.mozilla.org/en-US/docs/Web/HTML/Element/hr


<hr>

### a - anchor tag
The anchor tag, used for linking to other pages. This tag should include an href attribute with the path to the page being linked (absolute or relative). For example:

< a href="https://algoexpert.io">AlgoExpert</ a>
Learn more: https://developer.mozilla.org/en-US/docs/Web/HTML/Element/a

<hr>

### em - emphasis tag
The emphasis tag, usually rendered as italics by default in the browser. For example:

< p>I < em>need</ em> to study!</ p>
Learn more: https://developer.mozilla.org/en-US/docs/Web/HTML/Element/em

<hr>

### str - strong tag
The strong tag, usually rendered as bold by default in the browser. For example:

< p>< strong>Note:</ strong> This is important!</ p>
Learn more: https://developer.mozilla.org/en-US/docs/Web/HTML/Element/strong