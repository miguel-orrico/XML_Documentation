# COSAS IMPORTANTES SOBRE XML  

---

## XML Introduction  

### Diferencias entre XML y HTML  

| XML | HTML |
| :--- | :--- |
| Sirve para guardar datos | Sirve para mostrar datos |
| Las etiquetas no están definidas | Las etiquetas están definidas |
| Sensible a mayúsculas | No sensible a mayúsculas |
| Reglas estrictas | Más flexible |
| Transporta y guarda datos | Estructura páginas web |

### Para qué se usa XML  

- Guardar datos  
- Pasar datos entre sistemas  
- Separar los datos de la forma en que se muestran  
- Compartir información organizada  

---

## XML Syntax  

- Debe haber **una sola raíz**  
- Todos los elementos deben tener cierre  

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

## XML Tree  

- XML tiene una estructura en forma de **árbol**  
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

## XML Elements  

- Son los bloques principales de XML  
- Pueden contener texto, otros elementos o atributos  
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

## XML Attributes  

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