---
layout: answer
title: The Absolute Basics 
---

<h2 id="hello">Display a message with minimal code</h2>

### The Code 

~~~ html
Hello, world!
~~~

Yes! html can be written without any html elements. As the document type is not specified, the browser will enter quirks mode. You can read more about this [here][htmlmodes]. If you are interested in XHTML however, you should know it is less lenient. It's worth looking into the [purpose of XHTML][xhtmlpurp].

### Page Preview
Hello, world!

<h2 id="doctype">Display "Hello, html5!" with a HTML5 doctype and root element</h2>

### The Code

~~~ html
<!DOCTYPE "html">

<html>
Hello, world!
</html>
~~~

### Page Preview

<div class="page-preview">
Hello, world!
</div>

<h2 id="multline">Display multiple lines of text</h2>

### The Code

~~~ html
<!DOCTYPE "html">

<html>
  The HTML element (or HTML root element) represents the root of an HTML document. All other elements must be descendants of this element.

  Since the element is the first in a document other than comments, it is called the root element. Although this tag can be implied, or not required, with HTML, it is required to be opened and closed in XHTML.
</html>
~~~

### Page Preview

<div class="page-preview">
The HTML element (or HTML root element) represents the root of an HTML document. All other elements must be descendants of this element.

Since the element is the first in a document other than comments, it is called the root element. Although this tag can be implied, or not required, with HTML, it is required to be opened and closed in XHTML.
</div>

[htmlmodes]:https://developer.mozilla.org/en-US/docs/Quirks_Mode_and_Standards_Mode
[xhtmlpurp]:http://diveintohtml5.info/past.html#xhtml