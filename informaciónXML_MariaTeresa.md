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
Is everything from (including) the element's **start** tag to (including) the element's **end** tag.

There are XML name rules, but the most important are:
* Element names **cannot** contain spaces
* Element names are case-sensitive
* Element names **must** start with a letter or underscore, but **cannot** start with the letters xml

**Tip!** Choose your naming style, and be consistent about it!
  
XML elements can be extended to carry **more** information.

## XML Attributes
XML elements can have attributes, just like HTML. They **must always** be quoted.

There are no rules about when to use attributes or when to use elements in XML.

Things to consider:
* attributes cannot contain multiple values (elements can)
* attributes cannot contain tree structures (elements can)
* attributes are not easily expandable (for future changes)

**IMPORTANT**: 
Metadata (data about data) should be stored as attributes, and the data itself should be stored as elements.



