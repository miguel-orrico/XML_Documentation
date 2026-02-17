# COSAS IMPORTANTES SOBRE XML

## ¿Qué es XML?

XML, which stands for eXtensible Markup Language, is a markup language designed to store and transport data in a structured and platform-independent way. One of its most important characteristics is that it is extensible. Unlike HTML, which has predefined tags such as &lt;p&gt; or &lt;div&gt;, XML allows you to create your own tags. This means you can design a structure that fits exactly the type of data you are working with, whether it is information about books, students, transactions, or configuration settings. That flexibility is one of its core strengths.

&lt;person&gt;
  &lt;name&gt;Mike&lt;/name&gt;
  &lt;age&gt;29&lt;/age&gt;
&lt;/person&gt;

## Plain text format
Another key characteristic of XML is that it is text-based. XML documents are plain text files, which makes them human-readable and easy to edit with any text editor. Because they are just text, they are independent of operating systems, hardware, and programming languages. An XML file created on Windows can be read on Linux or macOS without modification. This portability is one of the reasons XML became widely used for data exchange between systems.

## Hierarchical Tree Structure
XML organizes data in a hierarchical tree structure. Every XML document must have exactly one root element, and inside that root, elements can contain other elements. This parent-child relationship forms a tree, where elements can have children, siblings, and nested levels. This hierarchical organization makes XML very suitable for representing structured and complex information.


## Strict Syntax Rules
Another defining feature of XML is that it is strict. XML has clear syntax rules that must be followed. All elements must be properly nested, every opening tag must have a corresponding closing tag (or be self-closing), tag names are case-sensitive, and attribute values must be quoted. If a document violates these rules, the XML parser will stop processing it. This strictness ensures consistency and reliability, especially when exchanging data between systems.

## Self-Descriptive
XML is also considered self-descriptive. The meaning of the data is conveyed by the tag names themselves. For example, &lt;price&gt; 29.99 &lt;/price&gt; clearly indicates what the value represents. This makes XML documents easier to understand without needing additional context.

## Supports Validation
Another important characteristic is that XML supports validation. Using tools like DTD or XML Schema (XSD), you can define the exact structure that an XML document must follow. You can specify which elements are allowed, which attributes are required, and even define data types. This allows systems to verify that incoming data follows a specific format before processing it.

## Separates Data from Presentation
Finally, XML focuses purely on describing information, not on how that information should look. Presentation can be handled by other technologies such as HTML, CSS, or XSLT. This separation makes XML useful in environments where the same data needs to be displayed in different ways.

## Resume
In short, XML is extensible, structured, strict, text-based, platform-independent, and capable of validation. It may not be the trendiest format today, but understanding XML gives you a strong foundation in how structured data works across systems.

## XML vs HTML
Diferences between XML and HTML
| XML | HTML |
| :--- | :--- |
| Designed to carry data | Designed to display data |
| Simplifies things | More complex |
| Does NOT do anything | Essential to show information |
| Tags not predefined | Tags predefined |

## XML VS JSON

Both XML and JSON are are text-based formats used to store and exchange structured data between systems that:

* Store structured data

* Send data between servers and clients

* Represent hierarchical information

* Serialize objects

So when you're building an API, designing a data format, or choosing how systems communicate, you have to decide which one fits better. That’s why the comparison matters.

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
