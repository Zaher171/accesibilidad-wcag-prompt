# Proceso de validacion WCAG 2.2

## Objetivo
Demostrar cumplimiento de criterios A y AA (AAA cuando aplique) para cada archivo en `corregido/`, comparando con `original/`.

## Herramientas minimas (usar al menos 3)
- WAVE
- Axe DevTools
- Lighthouse
- Accessibility Insights

## Flujo por archivo
1. Abrir archivo `original/*.html` en navegador.
2. Ejecutar WAVE, Axe y Lighthouse.
3. Guardar capturas "before" en `evidencias/screenshots/`.
4. Abrir archivo `corregido/*.html`.
5. Repetir validaciones.
6. Guardar capturas "after".
7. Completar tabla de resultados.

## Tabla de resultados
| Archivo | Herramienta | Antes (errores) | Despues (errores) | Estado final |
|---|---|---:|---:|---|
| index-formulario.html | WAVE | pendiente | pendiente | pendiente |
| index-formulario.html | Axe | pendiente | pendiente | pendiente |
| index-formulario.html | Lighthouse | pendiente | pendiente | pendiente |
| index-tabla.html | WAVE | pendiente | pendiente | pendiente |
| index-tabla.html | Axe | pendiente | pendiente | pendiente |
| index-tabla.html | Lighthouse | pendiente | pendiente | pendiente |
| index-media.html | WAVE | pendiente | pendiente | pendiente |
| index-media.html | Axe | pendiente | pendiente | pendiente |
| index-media.html | Lighthouse | pendiente | pendiente | pendiente |

## Checklist A/AA/AAA
- [ ] 1.1.1 Contenido no textual (A)
- [ ] 1.3.1 Info y relaciones (A)
- [ ] 1.3.2 Secuencia significativa (A)
- [ ] 1.4.1 Uso del color (A)
- [ ] 1.4.3 Contraste minimo (AA)
- [ ] 1.4.6 Contraste mejorado (AAA, objetivo)
- [ ] 2.1.1 Teclado (A)
- [ ] 2.4.1 Evitar bloques (A)
- [ ] 2.4.3 Orden de foco (A)
- [ ] 2.4.7 Foco visible (AA)
- [ ] 2.4.11 Foco no oculto (AA)
- [ ] 3.3.2 Etiquetas o instrucciones (A)
- [ ] 4.1.2 Nombre, funcion, valor (A)

## Evidencias esperadas
- `wave-before-*.png` / `wave-after-*.png`
- `axe-before-*.png` / `axe-after-*.png`
- `lighthouse-before-*.png` / `lighthouse-after-*.png`
- `accessibility-insights-before-*.png` / `accessibility-insights-after-*.png`

## Criterio de aprobacion
- 0 errores criticos en WAVE y Axe para A/AA.
- Lighthouse Accessibility >= 95.
- Riesgos AAA documentados por criterio (cumple/no aplica).
