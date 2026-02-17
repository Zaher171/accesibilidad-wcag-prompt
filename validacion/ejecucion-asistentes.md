# Ejecucion del prompt en multiples asistentes

## Objetivo
Comparar la eficacia del mismo prompt en distintos asistentes sin encadenar prompts.

## Asistentes
- GitHub Copilot (VS Code)
- Gemini (web)
- (Opcional) otro asistente compatible

## Regla de prueba
- Una corrida por archivo sobre HTML original.
- Si falla AA, volver al archivo original, ajustar prompt y repetir corrida completa.
- No corregir manualmente entre prompts para no sesgar resultados.

## Procedimiento estandar
1. Abrir `original/index-formulario.html`.
2. Copiar `prompts/prompt-perfecto.md` y pegarlo en el asistente.
3. Solicitar salida en reemplazo completo del HTML.
4. Guardar salida como `corregido/index-formulario.html`.
5. Repetir para `index-tabla.html` y `index-media.html`.
6. Validar con WAVE, Axe y Lighthouse.
7. Guardar evidencias antes/despues.

## Registro de resultados
| Asistente | Archivo | Errores WAVE despues | Errores Axe despues | Lighthouse accesibilidad | Cumple A/AA |
|---|---|---:|---:|---:|---|
| Copilot | index-formulario.html | pendiente | pendiente | pendiente | pendiente |
| Copilot | index-tabla.html | pendiente | pendiente | pendiente | pendiente |
| Copilot | index-media.html | pendiente | pendiente | pendiente | pendiente |
| Gemini | index-formulario.html | pendiente | pendiente | pendiente | pendiente |
| Gemini | index-tabla.html | pendiente | pendiente | pendiente | pendiente |
| Gemini | index-media.html | pendiente | pendiente | pendiente | pendiente |

## Criterio para elegir "prompt perfecto"
- Mayor tasa de cumplimiento A/AA en primera corrida.
- Menor numero de warnings recurrentes.
- Menor necesidad de post-edicion manual.
- Mejor trazabilidad del cambio por criterio WCAG.
