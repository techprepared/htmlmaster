# HTML Essential training

## 1 HTML intro
- HTML - Hypertext Markup Language
- It is a markup intended for the browser as the user don't see the tags and attributes so it is more important to browsers, yet we need to carefully communicate our messages to be understood
- For styling use CSS
- For interactivity use Javascript
- HTML is intended for all type of devices and systems
- HTML is simple markup language with no programming logic associated
- forgiving language which works even with mistakes, can take a lot of abuse
- CSS is a bit more fragile and a bit more powerful, if selector is wrong it is ignored
- Javascript is the more powerful and more fragile, if errors a page will break
- HTML, CSS, Javascript => resilience, robustness and power
- if you can put something in HTML then use HTML, if you can't use CSS and JS
## 2 Formatting text
- __use opening and closing tag__ to close element, not every element needs to be closed anymore
- __elements can be nested__, paring, children, siblings
- __Document Object Model DOM__ tree name is used
- [paragraph element demo on codepen.io](https://codepen.io/jensimmons/pen/bGbooGB)
- __headlines__ are important to identify different sections of a page, h1 tag most important, h6 the less important
- [demo of the headlines](https://codepen.io/jensimmons/pen/aboLEwE), h1 is the main title, h2 is the subtitle, don't pick headline based on how it looks but go for the meaning of the content
- headlines are important for screen readers
- look for 'design systems' and ways how the meaning for bigger and content rich websites are defined
- __important and emphasized__ => `em, strong, i, b` - forget `i, b` as you can always markup text with css as you like, if you want to convey something as strong use strong tag and you want to emphasize something use em
- strong => importance, seriousness, urgency
- em => emphasis, clarification, highlight, emotional nuance
- it is important to markup these elements correctly for people listening to our content
- __Lists__: to do lists, recipe lists, wishlist, bucket lists, but also navigation
- three kinds: unordered list, ordered list, definition list
- ul and ol uses li elements
- dl - definition lists and you have dt definition term inside with one or more dd definition description or data at the same level
- demo of lists [different lists on codepen.io](https://codepen.io/jensimmons/pen/eYOyoJO), can change the layout of the lists, also the numbering scheme
- __Quotes__: distinguish from the surrounding text, you have `blockquote` for block type quotation and `q` for inline elements
- inline elements are flowing with the text and they don't start new line, block level elements are starting a new line and can have width and height
- __Dates__: one element `time` with `datetime` attribute, not visible for users but mark the time for computers and search engines
- many possibilities with `time`, need to check the documentation, look at the [MDN Time element reference](https://lnkd.in/g7eqZhE)
- __code, pre, br__ elements: when you want to display HTML element on page but don't want to render it as actual element of the page itself you use HTML entities or `&somethinghere;` to mark it up
- [example poem problem](https://codepen.io/jensimmons/pen/VwZQBvJ) - this is the classic poem problem when you want to display a text by respecting the new lines in it
- if you want to display the text with all of the white space respected you use `pre` tag to enclose it [pre and code example](https://codepen.io/jensimmons/pen/gOYvjpa)
- __superscript, subscript and small text__ : subscript like in H<sub>2</sub>O formula and on the other side if mathematical expression for example x<sup>2</sup> and also footnotes<sup>[3]</sup>
- here is [example on codepen](https://codepen.io/jensimmons/pen/LYPQdMV)
- for `small` you can use it to markup small print like in legal documents, frequently used in copyright information for example
## 3 Understanding the power of HTML
- [some code to investigate with Inspector](https://codepen.io/jensimmons/pen/xxKjYRR) - on each browser you invoke Inspector with `ctrl+shift+I`, look at the tab `Elements`
- good idea is to investigate code from other websites to see how people are using elements and tags
- __HTML attributes__ : global and local attributes, common global are: class, id, lang, dir and many more
- __ARIA roles__ : for accessibility situations, provide accessible information about a specific element
- __Formatting HTML__ : comments, you have block comments and inline comments, the closing slash is not needed for some elements like img, br, hr, input and else
- __Weird characters__ : also called entities, you have `&nbsp;` which means non breaking space you mark a place where you want the text to stay together, opposite is `<wbr>` where the text if needed breaks at this place, but if you want the text to break with a dash indicating that the word on the next line is part of the previous word you use `&shy;` 