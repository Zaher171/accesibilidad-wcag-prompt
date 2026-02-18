Perfecto 💪
Te preparo un **README profesional, bien estructurado y listo para entrega**, alineado con una práctica de accesibilidad WCAG 2.2 y preparado para que pegues tus capturas.

Puedes copiar y pegar directamente:

---

# 🧩 Proyecto de Mejora de Accesibilidad – WCAG 2.2

## 📌 Descripción

Este proyecto consiste en la evaluación y mejora de la accesibilidad web de tres páginas HTML, aplicando criterios de las **WCAG 2.2** y validando los resultados mediante herramientas automáticas de auditoría.

Las páginas analizadas son:

* 📄 `index-formulario.html`
* 📰 `index-media.html`
* 📊 `index-tabla.html`

El objetivo ha sido detectar problemas de accesibilidad, corregirlos y comparar los resultados **antes y después** de las mejoras.

---

# 🛠 Herramientas de validación utilizadas

Se han utilizado las siguientes herramientas profesionales de auditoría:

* **WAVE (WebAIM)** – Análisis estructural y semántico
* **axe DevTools** – Detección automática de problemas WCAG
* **Google Lighthouse** – Puntuación global de accesibilidad

---

# 📄 1. Formulario – `index-formulario.html`

## 🔍 Problemas detectados (ANTES)

* Inputs sin etiquetas asociadas correctamente.
* Falta de atributo `lang` en el documento.
* Objetivos táctiles demasiado pequeños.
* Problemas de contraste.
* Falta de asociaciones ARIA.

---

## 🔴 Evidencias – Antes de las mejoras

### WAVE

<img width="1917" height="1015" alt="wave-before-formulario" src="https://github.com/user-attachments/assets/1c223107-653f-4ca4-ac6e-e7835097c132" />


### axe DevTools

![axe-before-formulario](./axe-before-formulario.png)

### Lighthouse

![lighthouse-before-formulario](./lighthouse-before-formulario.png)

---

## ✅ Mejoras aplicadas

* Asociación correcta de `<label>` con `for` e `id`.
* Inclusión del atributo `lang="es"` en `<html>`.
* Mejora de contraste de texto.
* Uso correcto de `aria-describedby`.
* Mejora del tamaño de botones y elementos interactivos.
* Uso semántico correcto de `fieldset` y `legend`.

---

## 🟢 Evidencias – Después de las mejoras

### WAVE

![wave-after-formulario](./wave-after-formulario.png)

### axe DevTools

![axe-after-formulario](./axe-after-formulario.png)

### Lighthouse

![lighthouse-after-formulario](./lighthouse-after-formulario.png)

---

# 📰 2. Noticias / Media – `index-media.html`

## 🔍 Problemas detectados (ANTES)

* Imágenes sin atributo `alt`.
* Bajo contraste de texto.
* Falta de landmark principal.
* Falta del atributo `lang`.
* Botones sin nombre accesible claro.

---

## 🔴 Evidencias – Antes de las mejoras

### WAVE

![wave-before-media](./wave-before-media.png)

### axe DevTools

![axe-before-media](./axe-before-media.png)

### Lighthouse

![lighthouse-before-media](./lighthouse-before-media.png)

---

## ✅ Mejoras aplicadas

* Inclusión de textos alternativos descriptivos en imágenes.
* Mejora del contraste de colores.
* Uso de `<main>` como landmark principal.
* Inclusión de `aria-labelledby` en botones.
* Corrección de jerarquía de encabezados (`h1`, `h2`).

---

## 🟢 Evidencias – Después de las mejoras

### WAVE

![wave-after-media](./wave-after-media.png)

### axe DevTools

![axe-after-media](./axe-after-media.png)

### Lighthouse

![lighthouse-after-media](./lighthouse-after-media.png)

---

# 📊 3. Tabla – `index-tabla.html`

## 🔍 Problemas detectados (ANTES)

* Tabla sin `caption`.
* Cabeceras sin definir correctamente (`<th>`).
* Falta de asociación semántica entre filas y columnas.
* Falta de landmark principal.
* Falta de atributo `lang`.

---

## 🔴 Evidencias – Antes de las mejoras

### WAVE

![wave-before-tabla](./wave-before-tabla.png)

### axe DevTools

![axe-before-tabla](./axe-before-tabla.png)

### Lighthouse

![lighthouse-before-tabla](./lighthouse-before-tabla.png)

---

## ✅ Mejoras aplicadas

* Inclusión de `<caption>` descriptivo.
* Uso correcto de `<th scope="col">` y `<th scope="row">`.
* Mejora de estructura semántica.
* Inclusión de `<main>`.
* Corrección del atributo `lang`.

---

## 🟢 Evidencias – Después de las mejoras

### WAVE

![wave-after-tabla](./wave-after-tabla.png)

### axe DevTools

![axe-after-tabla](./axe-after-tabla.png)

### Lighthouse

![lighthouse-after-tabla](./lighthouse-after-tabla.png)

---

# 📈 Comparativa de resultados

| Página     | Antes                         | Después                 |
| ---------- | ----------------------------- | ----------------------- |
| Formulario | Problemas críticos detectados | Sin errores automáticos |
| Media      | Errores de contraste y alt    | Validación limpia       |
| Tabla      | Estructura incompleta         | Semántica correcta      |

---

# 🎯 Criterios WCAG 2.2 trabajados

* 1.1.1 Contenido no textual
* 1.3.1 Información y relaciones
* 1.4.3 Contraste mínimo
* 2.4.6 Encabezados y etiquetas
* 3.3.2 Etiquetas o instrucciones
* 4.1.2 Nombre, función y valor

---

# 🧠 Conclusión

Tras aplicar las mejoras:

* Se eliminaron los errores automáticos detectados.
* Se mejoró la semántica del HTML.
* Se optimizó la experiencia para usuarios de lectores de pantalla.
* Se alineó el proyecto con los principios de accesibilidad WCAG 2.2.

La validación automática confirma la mejora, aunque siempre se recomienda realizar pruebas manuales complementarias.

---

# 📂 Convención de nombres de capturas

```
wave-before-formulario.png
wave-after-formulario.png
axe-before-formulario.png
axe-after-formulario.png
lighthouse-before-formulario.png
lighthouse-after-formulario.png
```

(Repetido para `media` y `tabla`)


