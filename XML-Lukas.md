# Introducción a XML

XML (eXtensible Markup Language) es un lenguaje de marcado diseñado principalmente para **almacenar y transportar datos**. A diferencia de HTML, que se centra en mostrar información en una página web, XML se enfoca en describir datos de forma estructurada para que puedan ser entendidos tanto por personas como por máquinas.

XML no fue creado para reemplazar otros lenguajes como JavaScript ni para diseñar interfaces visuales. Su propósito es servir como un formato estándar para el intercambio de información entre diferentes sistemas.



## ¿Cómo almacena los datos XML?

Una de las características más importantes de XML es que almacena la información en **texto plano**. Esto significa que:

- Puede abrirse con cualquier editor de texto.
- Es legible por humanos.
- Puede procesarse fácilmente por programas y aplicaciones.
- No depende de formatos binarios ni propietarios.

Gracias a esto, XML es muy flexible y ampliamente compatible.



## Independencia de plataforma

XML es **independiente del software y del hardware**. Esto quiere decir que:

- No está ligado a un sistema operativo específico.
- Puede utilizarse en distintas plataformas (Windows, Linux, macOS).
- Permite intercambiar datos entre aplicaciones desarrolladas en distintos lenguajes de programación.

Esta independencia es una de las razones por las que XML se convirtió en un estándar para el intercambio de datos en internet y en sistemas empresariales.



## Legibilidad: humanos y máquinas

Los documentos XML están diseñados para ser:

- **Comprensibles para las personas**, gracias a su estructura clara y etiquetas descriptivas.
- **Procesables por máquinas**, ya que siguen reglas sintácticas estrictas que permiten a los programas interpretarlos correctamente.

Esto facilita la comunicación entre diferentes sistemas informáticos y también permite que los desarrolladores puedan revisar los datos fácilmente.



## Idea principal de XML

La idea central detrás de XML es proporcionar una forma estructurada, clara y estandarizada de representar información. Su objetivo fundamental es permitir que los datos puedan almacenarse y transportarse de manera segura y comprensible entre distintos entornos tecnológicos.

---

# Sintaxis de XML 
Todos los documentos de XML deben de tener si o si exactamente un elemento root el cual debe de contener todos los demas elementos del documento.



## Prologo
No es obligatorio en un documento XML pero si existe debe de ser lo primero que hay en eel documento.

Los documentos XML pueden contener caracteres en Noruego o Frances que no se encuentran en otras lenguas por lo que se recomienda especificar el 'encoding'.

El 'encoding' por defecto es el internacional, expresado como 'UTF-8' que contiene los caracteres comentados con anterioridad.



## Especificaciones sobre la sintaxis de XML

- Todos los elementos deben de tener una etiqueta de cierre (o deben de ser auto concliusivas).
- Las etiquetas de XML son sensibles a las mayusculas y minusculas
- Las etiquetas deben de estar correctamente anidadas es decir `<b><i> texto </i></b>`
-En XML los atributos deben de estar siempre entre comillas por ejemplo:
```
<note date="12/11/2007">
  <to>Tove</to>
  <from>Jani</from>
</note>
```

---

# XML Structure
- Todos los documentos XML estan estructurados en forma de arbol (como uno genealogico).

- Todos tienen un elemento root del cual salen los hijos y sub hijos, todos los elementos pueden tener sub elementos(child elements).

- Los terminos Parent, child y sibling son utilizados para hacer referencia a las relaciones entre elementos .

---

# Elementos de XML

