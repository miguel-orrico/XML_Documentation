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
* XML documents must have **one** *root* element (parent)
* The *XML prolog* is optional. If it exists, it must come first in the document.
* All elements *must* have closing tag.
* Tags ***are case*** *sensitive*.
* All elements *must* be properly nested.
* In XML, an error in the document typically causes the parser to *STOP* processing.

## XML VS JSON

### 1. Basic Philosophy

#### XML

* Markup-based.
* Tag-driven.
* Hierarchical tree structure.

#### JSON

* Data-object based.
* Key–value structure.
* Maps directly to programming objects.

### 2. Readability

* JSON → shorter, cleaner, easier for humans.
* XML → more verbose, more structured, more formal.
* XML repeats tag names.
* JSON avoids duplication.
* Your eyes will thank JSON.

### 3. Strictness

* Both are strict formats.
* But XML is strict in a more ceremonial way:

#### XML
* Closing tags required
* Case sensitive
* Proper nesting required
* Attribute quoting mandatory

#### JSON:

* Uses braces {} and brackets []
* Strict commas
* Double quotes required for keys
* Both will break if malformed.

### 4. Structure Model

#### XML:

* Pure tree structure
* Uses elements and attributes
* Mixed content possible (text + elements)

#### JSON:

* Objects and arrays
* Naturally maps to dictionaries and lists
* no attributes concept
* JSON maps better to programming languages.

Hola
