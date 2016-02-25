---
layout: solution
title: The Absolute Basics
---

Absolute Basics | Answers
=========================

<h2 id="hello">Display a message with minimal code</h2>

{% include pen.html add="OMBovE" h=80 %}

What is this? HTML can be written without markup? Not exactly. The document type is not specified in the source for this solution, leaving the browser to enter [quirks mode][htmlmodes]. In quirks mode, the browser does the best it can to correctly display your page, with the markup you've provided. In future solutions I specify ```<!DOCTYPE html>``` in the source code, which is for HTML5 documents.

If you specify a certain variant of HTML, such as XHTML, you may be forced to write [well-formed][xhtmllen] markup. It's worth looking into the [purpose of XHTML][xhtmlpurp] for more background on this issue of well-formedness.


<h2 id="doctype">Greet HTML5, specifying a doctype and root element</h2>

{% include pen.html add="WrPboE" h=150 %}

The root element ```<html>``` surrounds all html source code besides the doctype. More elements such as ```<head>```, ```<body>``` and ```<p>``` should definitely be specified, and will be covered in later exercises.

<h2 id="multline">Write some paragraphs in a webpage</h2>

{% include pen.html add="XXOXGL" h=400 %}

Whitespace formatting is ignored in HTML5, and hence even though I wrote two paragraphs of text, the resulting webpage contains a single paragraph, with none of the indentation. Indentation can be added with elements such as paragraph ```<p>``` and unordered list ```<ul>```.

<h2 id="messline">Choose a program from <a href="https://en.wikibooks.org/wiki/Computer_Programming/Hello_world">here</a> and copy it into a webpage.</h2>

{% include pen.html add="qbgQGJ" h=300 %}

Here I've written a simple golang program in my HTML document. Clearly all the formatting has been removed, reinforcing what was said in the previous example.

Absolute Basics | Advanced Questions
====================================

<h2 id="versions">Write a webpage in a bunch of HTML variants</h2>

<h2 id="essential">Write a webpage with the essentials</h2>

{% include pen.html add="YwovZo" h=250 %}

This an inherently subjective question, to an astronomical degree. The code chosen was source from articles from places like 

[golangintro]: https://tour.golang.org/welcome/1
[htmlmodes]:https://developer.mozilla.org/en-US/docs/Quirks_Mode_and_Standards_Mode
[xhtmlpurp]:http://diveintohtml5.info/past.html#xhtml
[xhtmllen]:https://www.w3.org/TR/xhtml1/#diffs
[codepen]: http://codepen.io/about/
