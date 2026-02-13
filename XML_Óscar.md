# COSAS IMPORTANTES SOBRE XML

## XML Introduction
Diferences between XML and HTML
| XML | HTML |
| :--- | :--- |
| Designed to carry data | Designed to display data |
| Simplifies things | More complex |
| Does NOT do anything | Essential to show information |
| Tags not predefined | Tags predefined |

## XML Tree
* XML Tree starts at a root element
* All elements can have sub elements
* XML Documents are formed as element trees
* The terms used are parent, child and siblings
* Siblings are children on the same level, branch from the parent

## XML Syntax
* XML documents must have one *root* element (parent)
* The *XML prolog* is optional. If it exists, it must come first in the document.
* All elements *must* have closing tag.
* Tags are case *sensitive*.
* All elements *must* be properly nested.
* In XML, an error in the document typically causes the parser to *STOP* processing.

## XML Elements
* Elements are the building blocks of XML.
* They can contain text, other elements (child elements), or both.
* Elements are defined by a start tag `<tag>` and an end tag `</tag>`.
* Empty elements can use the self-closing form: `<tag/>`.
* Example:
```xml
<book>
    <title>XML Fundamentals</title>
    <author>John Doe</author>
</book>
```
## XML Attributes
* Attributes provide additional information about elements.
* They appear inside the start tag in name="value" form.
* An element can have multiple attributes, separated by spaces.
* Attribute values must always be quoted (single or double quotes).
* Example:
```xml
<book genre="Programming" language="English">
    <title>XML Fundamentals</title>
    <author>John Doe</author>
</book>
``` 