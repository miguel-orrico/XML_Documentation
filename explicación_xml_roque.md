# What is XML?
***
## XML is a type of file that is used for *data storage and transfer*, making it **readable** for the people.
## It ***must*** have: 
- A "root element".
- Closed tags (tags properly nested).

## It may have:
- Another elements (childs or siblings).
- Attributes to add more information.
- Prolog (a line that specifies the encoding used and the XML version).

# IMPORTANT
- The Metadata information goes to attributes, not to elements.
- Try not to use as many attributes, as they aren't as scalable as elements.

## The *main differences* we can observe are:
***
### For example, a comparison with HTML.
|| XML | HTML |
|----------|----------|----------|
|Introduction| Easy to understand, only for data storage and transfer | Has a lot of tags, attributes and is the most common thing in all pages |
|Syntax| You can put whatever name tag you want, but it must have a root element and closing tags | Has to be structured, with semantic meaning, opening and closing tags and you can include classes and ids |
|Elements| An element is everything that starts by the `<element>` starting tag and the `</element>` closing tag | The elements are structured, and could have for example an element surrounded by a `<div>` (another element)|
|Attribute| XML uses this to provide "extra information", instead of more `<elements>` | HTML tags can have a lot of attributes, and each one can have more than one, for example one `<section>` could have a class and an id at the same time, used for applying multiple CSS styles|
***
## What can be used for?. 
- A company that has resources and wants the data structured and organized.

- The company could use XML for storing and sending data.

- The company would add the main tags, such as the root element, and then add the correct tags to structure the data.

- The company could add attributes to add extra information and/or sibling or child elements to make data more clear.
***
## AN USAGE EXAMPLE (FOR EXAMPLE, A HOTEL)
`<hotel stars="5">`

`   <bigrooms id="1">`
`   <price>99.99</price>`
`   <capacity>5</capacity>`
`   </bigrooms>`

`   <mediumrooms id="2">`
`   <price>49.99</price>`
`   <capacity>2</capacity>`
`</mediumrooms>`

`<hotel>`

### As we can see, the data is clearly readable and is well structured (it has a root element and tags properly nested).
***

# What is XHTML?

## XHTML is a stricter version of HTML, designed for including XML in HTML and is supported by a big variety of browsers.

### Differences between XHTML and HTML:

- Must include the `xmlns` attribute on the `<html>` tag.
- Must include the DOCTYPE tag.
- Must have properly nested and closed tags.
- Must have `<html>`, `<head>` , `<title>` and `<body>`.
- Must have quoted values.

### XHTML won't display the website if there is any error, unlike HTML that will display it.