---
layout: solution
title: The Absolute Basics
---

<h2 id="hello">Display a message with minimal code</h2>

{% include pen.html add="OMBovE" h=80 %}

Oh what is this? HTML can be written without markup? Well... not exactly. The document type is not specified in the source for this solution, and so the browser will enter [quirks mode][htmlmodes]. You aren't using any specific version of HTML, as no  ```!DOCTYPE``` (document type) is specified, and so the browser does the best it can to correctly display your page with the markup you've provided. Interestingly, [CodePen][codepen], which I'm using to display source code, doesn't want us to bother including the document type, but for the educational benefit, we include the HTML5 doctype: ```<!DOCTYPE html>```, where appropriate in other solutions.

If you specify a certain variant of HTML, such as XHTML, you may be forced to write [well-formed][xhtmllen] markup. It's worth looking into the [purpose of XHTML][xhtmlpurp] for more background on this issue of well-formedness.


<h2 id="doctype">Greet HTML5, specifying a doctype and root element</h2>

{% include pen.html add="WrPboE" h=150 %}

You may notice the font is different between this solution and the one above it. This is because this answer has the text we wish to display surrounded by this: ```<html></html>```, and [CodePen][codepen] decides this is HTML5 with no formatting, so chooses to use a sans-serif font. The first solution is just plain text in a HTML document, and since [CodePen][codepen] isn't sure what we want, it displays the text in a sans font.

<h2 id="multline">Write some paragraphs in a webpage</h2>

{% include pen.html add="XXOXGL" h=400 %}

Whitespace formatting is ignored in HTML5, and hence even though I wrote two paragraphs of text, the resulting webpage contains a single paragraph, with none of the indentation. Indentation can be added with elements such as paragraph ```<p>``` and unordered list ```<ul>```.

<h2 id="messline">Write some paragraphs in a webpage.</h2>

{% include pen.html add="qbgQGJ" h=300 %}

Here I've written a simple golang program in my HTML document. Clearly all the formatting has been removed, reinforcing what was said in the previous example.

<h2 id="essential">Write a webpage with the essentials</h2>

{% include pen.html add="YwovZo" h=250 %}

This a very subjective question, but what I have written I believe correct.

[golangintro]: https://tour.golang.org/welcome/1
[htmlmodes]:https://developer.mozilla.org/en-US/docs/Quirks_Mode_and_Standards_Mode
[xhtmlpurp]:http://diveintohtml5.info/past.html#xhtml
[xhtmllen]:https://www.w3.org/TR/xhtml1/#diffs
[codepen]: http://codepen.io/about/
