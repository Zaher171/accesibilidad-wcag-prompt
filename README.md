# Proyecto: Prompt para Accesibilidad Web WCAG 2.2

## Objetivo (ES)
Construir y validar un prompt unico y reutilizable para asistentes de programacion (GitHub Copilot, Gemini, etc.) que transforme HTML no accesible en HTML accesible alineado con WCAG 2.2 (A y AA; AAA como objetivo adicional cuando aplique).

## Objective (EN)
Build and validate a single reusable prompt for coding assistants (GitHub Copilot, Gemini, etc.) to transform non-accessible HTML into accessible HTML aligned with WCAG 2.2 (A and AA; AAA as an additional target where applicable).

## Estructura del repositorio
- `original/`: HTML de partida con problemas de accesibilidad.
- `corregido/`: HTML corregido con semantica, ARIA y mejoras de teclado/contraste.
- `prompts/prompt-perfecto.md`: prompt final listo para usar en Copilot/Gemini.
- `validacion/proceso-validacion.md`: plan de pruebas y checklist con WAVE, Axe, Lighthouse, Accessibility Insights.
- `evidencias/screenshots/`: capturas antes/despues de cada herramienta.

## Archivos incluidos
- Originales:
  - `original/index-formulario.html`
  - `original/index-tabla.html`
  - `original/index-media.html`
- Corregidos:
  - `corregido/index-formulario.html`
  - `corregido/index-tabla.html`
  - `corregido/index-media.html`

## Prompt final
El prompt final se encuentra en `prompts/prompt-perfecto.md` e incluye:
- criterios WCAG 2.2 por niveles,
- reglas ARIA,
- semantica HTML5,
- teclado (`tabindex`, foco, orden logico),
- contraste y estados,
- formato de salida estricto,
- checklist de autovalidacion.

## Proceso de desarrollo del prompt (ES)
1. Se parte de tres paginas HTML con errores frecuentes (formularios sin `label`, tablas sin `caption` ni `scope`, imagenes sin `alt`, uso excesivo de `div`, enlaces ambiguos, foco no visible).
2. Se diseña un prompt inicial con instrucciones de semantica + ARIA + teclado + contraste.
3. Se ajusta el prompt para exigir salida estructurada y trazabilidad por criterio WCAG.
4. Se consolida el prompt final en formato robusto y reutilizable para distintos asistentes.

## Prompt development process (EN)
1. Start from three HTML pages with common accessibility defects (forms without labels, tables without caption/scope, missing alt text, div-only layout, ambiguous links, invisible focus).
2. Draft an initial prompt covering semantic HTML + ARIA + keyboard + contrast.
3. Refine prompt to enforce strict output and WCAG traceability.
4. Finalize a robust reusable prompt for multiple assistants.

## Pasos de validacion de accesibilidad (ES)
1. Ejecutar validacion *ANTES* sobre `original/`.
2. Aplicar el prompt en Copilot/Gemini para generar version corregida.
3. Ejecutar validacion *DESPUES* sobre `corregido/`.
4. Guardar capturas en `evidencias/screenshots/`.
5. Registrar resultados en `validacion/proceso-validacion.md`.
6. Si hay fallos AA, volver al original, ajustar prompt y repetir corrida unica.

## Accessibility validation steps (EN)
1. Run *BEFORE* validation on `original/` files.
2. Apply prompt in Copilot/Gemini to generate corrected output.
3. Run *AFTER* validation on `corregido/` files.
4. Save screenshots in `evidencias/screenshots/`.
5. Log findings in `validacion/proceso-validacion.md`.
6. If AA fails, reset to original, adjust prompt, rerun one-shot generation.

## Herramientas de validacion requeridas
- WAVE
- Axe DevTools
- Lighthouse
- Accessibility Insights
- (Opcional) ANDI, ARC Toolkit, Access Assistant

## Problemas tipicos y soluciones aplicadas
- Falta de etiquetas: agregar `label for` y `id` unicos.
- Jerarquia de encabezados rota: usar secuencia logica `h1 > h2 > h3`.
- Controles sin nombre accesible: usar texto visible, `aria-label` o `aria-labelledby` solo cuando necesario.
- Tabla sin contexto: agregar `caption`, `thead`, `th scope`.
- Teclado: foco visible, sin `tabindex` positivo, orden natural del DOM.
- Contraste: cumplir minimo 4.5:1 para texto normal (AA) y 7:1 para objetivo AAA.

## Evidencias de validacion
Agrega tus capturas aqui (ejemplos de nombre):
- `evidencias/screenshots/wave-before-formulario.png`
- `evidencias/screenshots/wave-after-formulario.png`
- `evidencias/screenshots/axe-before-tabla.png`
- `evidencias/screenshots/axe-after-tabla.png`
- `evidencias/screenshots/lighthouse-before-media.png`
- `evidencias/screenshots/lighthouse-after-media.png`

## Nota importante
En este entorno se preparo todo el repositorio y los archivos de prueba. La ejecucion de extensiones de navegador y captura de pantalla debe hacerse localmente en tu navegador/IDE.

## Crear repositorio en GitHub
1. Inicializar git (ya hecho localmente):
   - `git init`
2. Primer commit:
   - `git add .`
   - `git commit -m "feat: prompt WCAG 2.2 + muestras HTML + guia de validacion"`
3. Crear repo remoto y subir:
   - `gh repo create accesibilidad-wcag-prompt --public --source . --remote origin --push`

## Criterio de aceptacion
- Sin errores criticos en WAVE y Axe.
- Lighthouse Accessibility >= 95 (ideal 100).
- Cumplimiento A y AA verificado en al menos 3 herramientas.
- AAA documentado como "cumplido" o "no aplicable" por criterio.
