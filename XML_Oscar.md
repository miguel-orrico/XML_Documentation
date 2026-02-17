# COSAS IMPORTANTES SOBRE XML  

---

## Introducción a XML  

### Diferencias entre XML y HTML  

| XML | HTML |
| :--- | :--- |
| Sirve para guardar datos | Sirve para mostrar datos |
| Las etiquetas no están definidas | Las etiquetas están definidas |
| Sensible a mayúsculas | No sensible a mayúsculas |
| Reglas estrictas | Más flexible |
| Transporta y guarda datos | Estructura páginas web |

---

## Para qué se usa XML  

- Guardar datos  
- Pasar datos entre sistemas  
- Separar los datos de la forma en que se muestran  
- Compartir información organizada  
- Usado en APIs, archivos de configuración o servicios web  

---

## Estructura de XML (Árbol)  

- Todo XML tiene un elemento **raíz**  
- Un elemento puede tener **hijos** (sub-elementos)  
- Los elementos que están al mismo nivel son **hermanos**  

### Ejemplo

```xml
<libreria>
    <libro>
        <titulo>XML Básico</titulo>
    </libro>
</libreria>
```

- `libreria` → raíz  
- `libro` → hijo de libreria  
- `titulo` → hijo de libro  

---

## Sintaxis de XML  

- Debe haber **una sola raíz**  
- Los elementos deben cerrarse siempre  

```xml
<ejemplo>Hola</ejemplo>
```

- Las etiquetas distinguen mayúsculas y minúsculas  
- Los elementos deben estar bien anidados  
- Los valores de los atributos deben ir entre comillas  

### Comentarios

```xml
<!-- Esto es un comentario -->
```

### Caracteres especiales

| Carácter | Cómo escribirlo |
|-----------|----------------|
| < | `&lt;` |
| > | `&gt;` |
| & | `&amp;` |
| " | `&quot;` |
| ' | `&apos;` |

---

## Elementos  

- Son los bloques principales de XML  
- Pueden tener texto, otros elementos o atributos  
- Los elementos vacíos se escriben así:

```xml
<br/>
```

### Ejemplo

```xml
<libro>
    <titulo>XML Básico</titulo>
    <autor>Óscar Valdivia</autor>
</libro>
```

---

## Atributos  

- Dan información extra a un elemento  
- Se escriben dentro de la etiqueta de inicio  
- Formato: `nombre="valor"`  

### Ejemplo

```xml
<libro genero="Programación" idioma="Español">
    <titulo>XML Básico</titulo>
    <autor>Óscar Valdivia</autor>
</libro>
```

---

## Namespaces (Opcional)  

- Sirven para evitar que se repitan nombres de etiquetas  

```xml
<h:tabla xmlns:h="http://www.w3.org/TR/html4/">
  <h:fila>
    <h:celda>Manzanas</h:celda>
  </h:fila>
</h:tabla>
```

---

## Validación (Opcional)  

- XML puede validarse con **DTD** o **XSD**  
- Esto ayuda a que el XML tenga la estructura correcta  

### Ejemplo DTD

```xml
<!DOCTYPE nota [
<!ELEMENT nota (para,de,cuerpo)>
<!ELEMENT para (#PCDATA)>
<!ELEMENT de (#PCDATA)>
<!ELEMENT cuerpo (#PCDATA)>
]>
```

---

## Bien formado vs Válido  

| Bien formado | Válido |
|--------------|--------|
| Sigue las reglas básicas de XML | Sigue reglas y estructura definida |
| Tiene una raíz | Cumple DTD o XSD |
| Etiquetas cerradas | Tipos de datos correctos |

> Todo XML válido está bien formado, pero no todo XML bien formado es válido.
