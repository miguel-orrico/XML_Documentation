# <span style="color:#1E90FF;">Introducción a XML</span>

XML (eXtensible Markup Language) es un lenguaje de marcado pensado **para almacenar y transportar información**.  
A diferencia de HTML, no se centra en cómo se muestra la información, sino en **qué representa**.  
Es independiente de plataformas y sistemas, y es una recomendación oficial del **W3C**.

---

## <span style="color:#32CD32;">¿Qué hace XML?</span>

- Permite organizar datos usando **etiquetas definidas por el autor**.  
- No ejecuta acciones; necesita un programa que interprete, envíe o muestre los datos.  
- Facilita el intercambio de información entre sistemas diferentes.  
- Es **flexible**: se pueden añadir o quitar elementos sin afectar a las aplicaciones existentes.

---

## <span style="color:#FF8C00;">XML vs HTML</span>

| Característica       | XML                              | HTML                               |
|----------------------|---------------------------------|-----------------------------------|
| Propósito             | Transportar y describir datos   | Mostrar datos en pantalla         |
| Etiquetas             | Definidas por el autor          | Predefinidas (`<p>`, `<h1>`, etc.) |
| Flexibilidad          | Extensible                       | Limitada, pensada para presentación |

---

## <span style="color:#8A2BE2;">Características principales</span>

- **Extensible:** puedes agregar etiquetas como `<date>` o `<hour>` sin romper programas existentes.  
- **Portátil:** se guarda en texto plano, independiente de sistemas y dispositivos.  
- **Compatible con muchos lectores:** humanos, computadoras, feeds, asistentes de voz, etc.  
- **Facilita la interoperabilidad** entre sistemas con formatos distintos.

---

## <span style="color:#DC143C;">Ejemplo básico</span>

```xml
<note>
  <to>Tove</to>
  <from>Jani</from>
  <heading>Recordatorio</heading>
  <body>¡No me olvides este fin de semana!</body>
</note>
