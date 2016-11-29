In all these examples there is a set of elements that span all of the language variants. Here's a breakdown:

1. **Document Type**: ```<!DOCTYPE ...>``` The document type is used by the page renderer to determine what version of HTML to expect in the document's source code. There is much more [anecdotal information][divequirks] swimming around in the ether, for those who have a wicked urge to delve into the dark, twisty depths of the doctype's history. Others who just want a [straightforward][htmlmodes] explanation may find [useful][w3forget] information around the web too, if you [dare][doctypesong] to look.
2. **Definition / Root:** ```<html> ... </html>``` The root tags specifies that the nested content of the element is html source code.
3. **Metadata:** ```<head> ... </head>``` Metadata is used to describe the content of a html document, such as the character set, content type and document title.
4. **Content:** ```<body> ... </body>``` What is displayed to the web user is the content of the webpage, which may consist of embedded content, text content or both, and is collectively referred to as [flow content][mdnflow].

[mdnflow]: https://developer.mozilla.org/en-US/docs/Web/Guide/HTML/Content_categories#Flow_content