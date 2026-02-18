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

<img width="1917" height="1015" alt="axe-before-formulario" src="https://github.com/user-attachments/assets/267e2317-5427-4441-81b5-478ac251b774" />


### Lighthouse

<img width="1917" height="1015" alt="lighthouse-before-formulario" src="https://github.com/user-attachments/assets/c5a0524d-4722-404f-8d0b-73c9a06bd3b1" />


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
<img width="1903" height="975" alt="wave-after-formulario" src="https://github.com/user-attachments/assets/04540f07-323a-4459-b2f9-029056aa2bd5" />

### axe DevTools

<img width="1899" height="1033" alt="axe-after-formulario" src="https://github.com/user-attachments/assets/33b0b888-0ecf-4413-afc5-f3ced61d248d" />


### Lighthouse

<img width="1912" height="965" alt="lighthouse-after-formulario" src="https://github.com/user-attachments/assets/1d3ab2e8-c858-4f8f-b0a3-419823df3e2f" />


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

<img width="1916" height="960" alt="wave-before-media" src="https://github.com/user-attachments/assets/1ca4330a-a04b-43a2-9f7d-e6b91b631be0" />


### axe DevTools

<img width="1916" height="960" alt="axe-before-media" src="https://github.com/user-attachments/assets/b7e6a9b7-13bb-4263-971d-0685074f8b38" />



### Lighthouse

<img width="1917" height="952" alt="lighthouse-before-media" src="https://github.com/user-attachments/assets/c702fbc5-9782-44c3-88d2-605027e5e1d5" />



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

<img width="1916" height="1019" alt="wave-after-media" src="https://github.com/user-attachments/assets/5badf7c3-1b4a-4fe6-9a62-42e9f53959c4" />


### axe DevTools

<img width="1913" height="1007" alt="axe-after-media" src="https://github.com/user-attachments/assets/831a64bb-24b4-401f-bd42-fc41e46aa395" />


### Lighthouse

<img width="1914" height="975" alt="lighthouse-after-media" src="https://github.com/user-attachments/assets/072e3a65-2e1b-459f-93af-5193fdf7b5db" />


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

<img width="1916" height="986" alt="wave-before-tabla" src="https://github.com/user-attachments/assets/04301250-2778-4ca1-b104-1701beee2fe0" />


### axe DevTools

<img width="1916" height="986" alt="axe-before-tabla" src="https://github.com/user-attachments/assets/7ce82899-546d-4af8-9688-7fc9c9238522" />


### Lighthouse

<img width="1919" height="955" alt="lighthouse-before-tabla" src="https://github.com/user-attachments/assets/48defe09-e566-445c-8c88-dbd0f86603b8" />


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

<img width="1915" height="1022" alt="wave-after-tabla" src="https://github.com/user-attachments/assets/037545f7-effc-409a-b319-49b2ab2df0fc" />


### axe DevTools

<img width="1904" height="1025" alt="axe-after-tabla" src="https://github.com/user-attachments/assets/4f17eb73-60df-4743-a730-8f44e93c8e50" />


### Lighthouse

<img width="1913" height="990" alt="lighthouse-after-tabla" src="https://github.com/user-attachments/assets/d2679d98-5245-4772-a534-98f6a3b57d31" />


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


