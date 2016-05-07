---
layout: solution
title: The Absolute Basics
quote: HTML should be considered an extension of punctuation.
qauth: Amittai Aviram
---

Absolute Basics | Answers
=========================

<h2 id="hello">Display a message with minimal code</h2>

{% include pen.html add="OMBovE" h=80 %}

What is this? HTML can be written without any markup elements! No, not exactly. The document type is not specified in the source for this solution, leaving the browser to enter [quirks mode][htmlmodes]. In quirks mode, the browser does the best it can to correctly display your page. In future solutions we specify ```<!DOCTYPE html>``` in the source code, which is the HTML5 document type.

If you specify a certain variant of HTML, such as XHTML, you may be forced to write [well-formed][xhtmllen] markup. It's worth looking into the [purpose of XHTML][xhtmlpurp] for more background on this issue of well-formedness.


<h2 id="doctype">Greet HTML5, specifying a doctype and root element</h2>

{% include pen.html add="WrPboE" h=150 %}

The root element, ```<html>```, surrounds all html source code besides the doctype. More elements such as ```<head>```, ```<body>```, and ```<p>``` should definitely be specified, and will be covered in later exercises.

<h2 id="multline">Write some paragraphs in a webpage</h2>

{% include pen.html add="XXOXGL" h=400 %}

Whitespace formatting is ignored in HTML5, such as the indentation and paragraphing in the above solution. Indentation can be added with elements such as paragraph ```<p>``` and unordered list ```<ul>```.

<h2 id="messline">Choose a program from the hello world <a href="https://en.wikibooks.org/wiki/Computer_Programming/Hello_world">wikibook</a>, and copy it into a webpage.</h2>

{% include pen.html add="qbgQGJ" h=300 %}

Here we've written a simple golang program in my HTML document. Clearly all the formatting has been removed, reinforcing what was said in the previous example.

Absolute Basics | Advanced Questions
====================================

<h2 id="versions">Write a very simple webpage in five different HTML versions</h2>

**NOTE:** This exercise is likely to be updated over time. Current solutions are drafts.

<h3 id="version5">HTML 5 Document</h3>
{% include pen.html add="PNBgyG" h=250%}

<h3 id="version4">HTML 4 Document</h3>
{% include pen.html add="KzxXgR" h=250%}

<h3 id="version3">HTML 3.2 Document</h3>

Coming Soon! Sorry this exercise is taking some time to research.

<h3 id="version2">HTML 2.0 Document</h3>

Coming Soon! Sorry this exercise is taking some time to research.

<h3 id="versionx">XHTML (Strict) Document</h3>
{% include pen.html add="JXaMZw" h=250 %}

In all these examples, a specific set of html tags, attributes and content span all of the language variants. Here's a breakdown:

1. **Document Type**: ```<!DOCTYPE ...>``` The document type is used by the page renderer to determine what version of HTML to expect in this document. There is much more [anecdotal information][divequirks] swimming around in the ether, for those who have a wicked urge to delve into the dark, twisty depths of the doctype's history. Others who just want a [straightforward][htmlmodes] explanation may find [useful][w3forget] information around the web too, if you [dare][doctypesong] to look.
2. **Definition / Root:** ```<html></html>``` Specifies that the nested content of the element is html source code.

...

More to come on this!

<h2 id="essential">Write a webpage with the essentials</h2>

{% include pen.html add="YwovZo" h=250 %}

This an inherently subjective question, to an astronomical degree. The code chosen was source from articles from places like

[golangintro]: https://tour.golang.org/welcome/1
[htmlmodes]:https://developer.mozilla.org/en-US/docs/Quirks_Mode_and_Standards_Mode "MDN: Quirky Standardy Discussion"
[xhtmlpurp]:http://diveintohtml5.info/past.html#xhtml "Dive Into HTML: XHTML"
[xhtmllen]:https://www.w3.org/TR/xhtml1/#diffs "W3C XHTML Comparison"
[codepen]: http://codepen.io/about/ "Codepen: This website's current saviour"
[divequirks]: http://diveintohtml5.info/semantics.html#the-doctype "Dive Into HTML: The Doctype"
[doctypesong]: http://learnhtmlwithsong.com/blog/13-doctype/ "Learn HTML with Song!"
[w3forget]: https://www.w3.org/QA/Tips/Doctype "W3C: Don't forget the doctype!"
