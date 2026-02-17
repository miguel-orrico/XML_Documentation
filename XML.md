# XML (eXtensible Markup Language)

XML es un lenguaje de marca (como html) en el cual se utiliza para almacenar datos. Las siglas XML significa Lenguaje de Marcado Extensible.

## Diferencias entre XML y HTML

XML está diseñado para transmitir y almacenar datos. Mientras que HTML esta diseñado para mostrar datos.

## Como usar XML

Si necesita mostrar datos en un documento HTML, dedicará mucho tiempo a editar el HTML cada vez que cambien los datos.

Con XML, los datos se pueden almacenar en un archivo XML independiente.

Con solo unas pocas líneas de código JavaScript, puede leer un archivo XML externo y actualizar el contenido de datos de su página web.

#### Ejemplo de w3school

```XML
<?xml version="1.0" encoding="UTF-8"?>
<bookstore>

  <book category="cooking">
    <title lang="en">Everyday Italian</title>
    <author>Giada De Laurentiis</author>
    <year>2005</year>
    <price>30.00</price>
  </book>

  <book category="children">
    <title lang="en">Harry Potter</title>
    <author>J K. Rowling</author>
    <year>2005</year>
    <price>29.99</price>
  </book>

  <book category="web">
    <title lang="en">XQuery Kick Start</title>
    <author>James McGovern</author>
    <author>Per Bothner</author>
    <author>Kurt Cagle</author>
    <author>James Linn</author>
    <author>Vaidyanathan Nagarajan</author>
    <year>2003</year>
    <price>49.99</price>
  </book>

  <book category="web" cover="paperback">
    <title lang="en">Learning XML</title>
    <author>Erik T. Ray</author>
    <year>2003</year>
    <price>39.95</price>
  </book>

</bookstore>
```

## XML Sintaxis

Todos los documentos XML deben tener un elemento root

```xml
<root>
    <parent>
        <child>
            .....
        </child>
    </parent>
</root>
```

# XML Tree

Los documentos XML estan estructurados en forma de arbol empezando por el root
