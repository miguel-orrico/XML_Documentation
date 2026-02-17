# XML

***

## What is XML?

XML is a software/hardware introduction tool for storing and transporting data.

***

## Why use XML?
* Does not use predefinded tags
* Is extensible, most XML applications will work even if new data is added or removed
* Simplifies things like:   
    * Data sharing
    * Data transport
    * Data availability
    * Platform independence

***

## XML Tree Structure
XML docs are formed as element trees.
The terms parent, child, and sibling are used to describe the relationships between elements.
* Parents have children. 
* Children have parents. 
* Siblings are children on the same level.

***

## XML Syntax Rules
* XML Prologue:
`<?xml version="1.0" encoding="UTF-8"?>`
* Closing tags: `<p>Hello World</p>` or `<br/>`
* Case sensitivity: `<p>` and `<P>` are different tags.
* Elements must be properly nested: `<p><b>Hello World</b></p>` is correct, but `<p><b>Hello World</p></b>` is not.
* Attribute values must be quoted: `<p id="text">`

***

## XML Elements and Attributes
### Elements
Elements are everything between the start and end tags. They can contain text, attributes, other elements, or all of that mixed.

A little example of how elements can be constructed:
`<message>`
`  <header>`
`    <from>Enzo</from>`
`    <to>Nahuel</to>`
`  </header>`
`  <body subject="presentation">Hello World</body>`
`</message>`

An empty element can be written as `<p/>` or `<p></p>`.

***

### Attributes
