# **XML Documentation**

## Collaborative Document about What's important in XML





### **XML (eXtensible Markup Language)**:

#### Fue diseñado para almacenar y transportar datos.


---
* ### **General**
---

**XML** surgió de la **necesidad de intercambiar datos y que fuese intelligible**. Por ello este **lenguaje** se encarga de **contener información** envuelto en etiquetas, las cuales no están predefinidas como HTML, sino que son inventadas por el autor del documento.



XML **simplifica** las cosas, haciendo que las **incompatibilidades** con el **transporte, compartir o incluso almacenaje de los datos se minimicen**. Lo que hace que sea más fácil el expandir o mejorar nuestras aplicaciones, páginas, etc. **sin perder esos datos**.


---
* ### **Usos**
---

XML **NO** define el cómo se muestran los datos. Lo que le permite que la misma información, como en el caso del tiempo que hace en Elche, se pueda mostrar de diversas maneras. Por ejemplo, una página web o aplicación móvil.


---
* ### **Estructura de árbol (Tree)**
---

Todo documento XML empieza **SIEMPRE** con al menos un **elemento raíz (root)**, del cual se despenden **elementos hijos** y de los cuales pueden contener aún más elementos, formando así unos **niveles jerárquicos**. Por ejemplo:



```

<root>

  <hijo\\\_1>

    <subhijo>...</subhijo>

  </hijo\\\_1>

  <hijo\\\_2>

    <subhijo>...</subhijo>

  </hijo\\\_2>

</root>

```


---
* ### **Sintaxis autodocumentada (Self-Describing Syntax)**
---


XML es **descriptivo por naturaleza**. Por ejemplo, en el caso de una librería:



`<?xml version="1.0" encoding="UTF-8"?>` **-> Prolog:** Se encarga de definir la versión y codificación de caracteres (Opcional, pero preferiblemente se tiene que usar)

```

<bookstore>

   <book category="cooking">

      <title>Everyday Italian</title>

      <author>Giada De Laurentiis</author>

      <year>2005</year>

      <price>30.00</price>

   </book>

</bookstore>

```



A partir de esta estructura se puede entender fácilmente que el documento contiene información sobre libros de una librería.


---
* ### **Otras características**
---


Aunque es cierto que se inventan las etiquetas existen **entidades predefinidas principalmente para caracteres especiales.** Por ejemplo:



|**`&lt;`**|**<**|**menos que**|
|-|-|-|
|**`&gt;`**|**>**|**mayor que**|
|**`&amp;`**|**\&**|**ampersand**|
|**`&apos;`**|**'**|**apostrofe**|
|**`&quot;`**|**<br />"**|**comillas**|



**Ej:**

`<message>salary < 1000</message>`

`<message>salary &lt; 1000</message>`





Además, para **comentar es similar a HTML:** `<!-- This is a comment -->`




---
* ### **Elementos y reglas del XML**
---


**Un elemento XML** comprende todo lo que va desde la etiqueta de apertura hasta la etiqueta de cierre. Destacando también los **elementos vacíos**, los cuales pueden tener atributos: <element></element>


---
### **Reglas de nombrado en XML:**
---

Los nombres de los elementos deben cumplir estas reglas:



* Son **sensibles** a **mayúsculas/minúsculas**.
* **Deben** comenzar con letra o guion bajo (_).
* **No** **pueden** comenzar con **"xml"** (en ninguna combinación de mayúsculas).
* **Pueden** contener **letras, números, guiones (-), guiones bajos (_), y puntos (.)**.
* **No pueden** contener **espacios**.
* **No** hay **palabras reservadas** (excepto "xml").




---
### **Cosas a tener en cuenta:**
---

No es obligatorio como las reglas, pero se deberían usar:



* Usar **nombres descriptivos y claros**: `<firstname>`, `<lastname>`.



* Mantenerlos **simples y concisos**.



* **Evitar**:



&emsp;&emsp; 	**-** (puede interpretarse como resta en algunos contextos).

&emsp;&emsp; 	**.** (puede interpretarse como propiedad de objeto).

&emsp;&emsp; 	**:** (reservado para namespaces).



Es **recomendable** elegir una convención y mantener consistencia:

* lower case → `<firstname>`
* UPPER CASE → `<FIRSTNAME>`
* snake\_case → `<first_name>`
* PascalCase → `<FirstName>`
* camelCase → `<firstName>`


---
### **Atributos en XML:**
---

Al igual que en HTML, XML pueden tener atributos que **proporcionan información adicional sobre un elemento.**

**PERO, no existen reglas de usar un atributo o elemento,** por lo tanto se pueden usar dependiendo del diseño del documento. Por ejemplo:



**ATRIBUTO**:



```

<person gender="female">

   <firstname>Anna</firstname>

   <lastname>Smith</lastname>

</person>

```



**ELEMENTO**:



```

<person>

   <gender>female</gender>

   <firstname>Anna</firstname>

   <lastname>Smith</lastname>

</person>

```

Aunque hay que tener en cuenta que los atributos **tienen limitaciones**:

* Los atributos **no pueden contener múltiples valores estructurados**.
* **No pueden contener subelementos** (estructura en árbol).
* Son **menos flexibles** ante cambios futuros.
* Un **uso excesivo** puede volver el documento **difícil de mantener**.
