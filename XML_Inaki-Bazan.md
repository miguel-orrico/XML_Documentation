
# XML Notes

## 1. Introduction

### What is XML?

XML stands for *eXtensive Marking Language*. It is designed to store and transport data, using natural language to be self-descriptive. However, XML by itselt has no functionality, and can only be used in relationship with other languages and systems.

### Contents of a XML file

```
<note>
  <to>Tove</to>
  <from>Jani</from>
  <heading>Reminder</heading>
  <body>Don't forget me this weekend!</body>
</note>
```

### Differences between XML and HTML

- XML is a language used to mark data, whereas HTML is used to *display* data in a structured way.
- HTML, contrary to XML, has predefined labels and attributes.

<hr>

## 2. XML Contents and Rules

### General Rules

- All XML elements must have a opening and closing tag (except self-closing ones).
- XML tags **must** be properly nested.
- XML tags are case sensitive (```<A>``` is different from ```<a>```).
- XML attributes must be indicated in value pairs (```name="Iñaki Bazán"```).
- White-spaces are not truncated like in HTML.

### The XML Prologue

```
<?xml version="1.0" encoding="UTF-8"?>
```

### Special Characters

| Code | Char | Meaning |
|:---:|:---:|:---:|
| ```&lt;``` | < | less than |
| ```&gt;``` | > | greater than |
| ```&amp;``` | & | ampersand |
| ```&apos;``` | ' | apostrophe |
| ```&quot;``` | " |quotation mark |

### Comments

```
<!-- This is a comment -->
<!-- This is an invalid -- comment -->
```

### Empty Elements / Self-Closing Tags

XML elements can be empty, and are treated as self-closing tags. These elements can still have attributes:

```
<element attr="something"></element>
<element attr="something">
```

<hr>

## 3. Naming Rules and Conventions

All XML element names must follow these rules:
- They have to start with a letter or an underscore character (```_```).
- They cannot start with ```XML``` or any lower-case combination (```xml```, etc.), as it is the only XML reserved word.
- They must not contain spaces.

### Best Naming Practices

- Create short, simple, self-descriptive names (```name``` or ```firstname``` instead of ```the_name_of_the_person```).
- Avoid ```-```, as the software might interpret that you want to subtract the elements in between.
- Avoid ```.```, as the software might interpret that you are trying to invoke a property of an object.
- Avoid ```:```, as they are reserved for namespaces.
- Even though some unicode characters are legal (```áèü```), they can produce errors with some software.

### Conventions for Naming by Letter Case

- Lower case: ```<firstname>```
- Upper case: ```<FIRSTNAME>```
- Camel case: ```<firstName>``` (commonly used in *Java* and *JavaScript*)
- Snake case: ```<first_name>``` (commonly used in *SQL* databases)
- Pascal case: ```<FirstName>``` (commonly used in the *C* language)

Choose a naming convention and use it consistently across your XML file. Some XML files are associated to a certain database and follow its naming rules and conventions.

## 4. XML Attributes

XML attributes are declared following these format: ```attr="value"```. They can use single or double quotes.

```
<person gender="female">
<person gender='nonbinary'>
```

Attributes can also use single quotes if they are surrounded by double quotes, and vice versa. They can also use the ```&apos;``` and ```&quot;``` character entities.

<hr>

There are no rules that encourage or dismiss either the use of elements (tags) or attributes:

```
<person gender="female">
  <firstname>Anna</firstname>
  <lastname>Smith</lastname>
</person>
```

```
<person>
  <gender>female</gender>
  <firstname>Anna</firstname>
  <lastname>Smith</lastname>
</person>
```

These two examples provide the same information. The fact that the person's gender is an element or an attribute does not change the information on the file, and it will only depend on the software that interprets the XML file.

### XML Attributes for Metadata

Elements can be assigned ID references. These IDs can be used just like HTML ones:
```
<note id="501">
    <to>Tove</to>
    <from>Jani</from>
    <heading>Reminder</heading>
    <body>Don't forget me this weekend!</body>
</note>
```

### Attributes overuse

NOT using attributes is recommended in favor of using elements (tags). This is because:
- Attributes cannot contain multiple values (elements can).
- Attributes are not able to form tree structures (elements can).
- Attributes are not easily expandable for future changes.

Avoid:

```
<note id="501" day="10" month="01" year="2008"
to="Tove" from="Jani" heading="Reminder"
body="Don't forget me this weekend!">
</note>
```

This causes less headaches:

```
<note id="501">
    <date>
        <day>10</day>
        <month>01</month>
        <year>2008</year>
    </date>
    <to>Tove</to>
    <from>Jani</from>
    <heading>
        Reminder
    </heading>
    <body>
        Don't forget me this weekend!
    </body>
</note>
```

