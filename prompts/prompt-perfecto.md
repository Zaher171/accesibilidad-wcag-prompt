# Prompt perfecto para asistentes de programacion (Copilot / Gemini)

## Contexto
Actua como especialista senior en accesibilidad web. Recibiras un archivo HTML con problemas de accesibilidad.
Tu objetivo es devolver una version corregida que cumpla WCAG 2.2 nivel A y AA (AAA cuando sea razonable y sin romper UX).

## Instrucciones obligatorias
1. Mantener funcionalidad original de la pagina.
2. Mejorar semantica HTML5 con landmarks: `header`, `nav`, `main`, `aside`, `section`, `article`, `footer`.
3. Corregir jerarquia de encabezados (`h1` unico por vista; niveles sin saltos).
4. Formularios:
   - Asociar cada campo con `label for` + `id` unico.
   - Usar `fieldset` + `legend` para grupos.
   - Marcar errores con texto visible y asociacion semantica (`aria-describedby`, `aria-invalid`).
   - No usar placeholder como sustituto de etiqueta.
5. Imagenes:
   - `alt` descriptivo para imagen informativa.
   - `alt=""` y `role="presentation"` solo en decorativas.
6. Enlaces y botones:
   - Nombre accesible claro y contextual.
   - Evitar textos ambiguos tipo "click aqui".
   - Usar `button` para acciones y `a` para navegacion.
7. Tablas:
   - Incluir `caption`.
   - Estructura con `thead`/`tbody`.
   - `th` con `scope` correcto.
8. Teclado y foco:
   - Navegable 100% por teclado.
   - Foco visible de alto contraste.
   - No usar `tabindex` positivo.
   - Solo usar `tabindex="0"` cuando sea necesario en elementos no nativos interactivos.
9. ARIA:
   - Regla principal: "No ARIA is better than bad ARIA".
   - Usar ARIA solo para complementar semantica nativa, no para reemplazarla.
   - Validar nombres, roles y estados (`aria-expanded`, `aria-controls`, `aria-live`, etc.) cuando aplique.
10. Color y contraste:
   - Texto normal >= 4.5:1 (AA), ideal 7:1 (AAA).
   - Texto grande >= 3:1 (AA).
   - Componentes UI y foco >= 3:1.
   - No depender solo del color para transmitir estado.
11. Idioma y metadatos:
   - Definir `lang` correcto en `<html>`.
   - Incluir `<meta charset="utf-8">` y viewport.
12. Patrones recomendados:
   - Agregar "skip link" al contenido principal.
   - Evitar `accesskey` salvo requerimiento explicito; si se usa, documentar conflicto potencial.
   - Incluir mensajes para lectores de pantalla cuando haya cambios dinamicos.

## Salida esperada (formato estricto)
Devuelve exactamente estas 3 secciones:

### 1) HTML corregido
Entrega el archivo HTML completo y valido.

### 2) Resumen de cambios
Lista de cambios con este formato por linea:
- `[WCAG criterio] Cambio aplicado - razon tecnica`
Ejemplo:
- `[1.1.1] Se agrego alt descriptivo a imagen principal - asegura alternativa textual`

### 3) Checklist de cumplimiento
Tabla Markdown con columnas:
- `Criterio`
- `Nivel (A/AA/AAA)`
- `Estado (Cumple/No cumple/No aplica)`
- `Evidencia en codigo`

## Restricciones
- No eliminar contenido funcional.
- No introducir dependencias JS/CSS externas salvo que se solicite.
- Mantener codigo legible e indentado.
- Priorizar HTML nativo sobre ARIA.

## Auto-verificacion final obligatoria
Antes de responder, revisa que:
- No existen inputs sin label.
- No hay imagenes sin alt.
- No hay salto incorrecto de encabezados.
- Todos los controles son accesibles por teclado.
- El foco visible esta implementado.
- El contraste minimo AA se cumple.

Si algo no puede garantizarse desde HTML puro (por ejemplo contraste de imagen de fondo), indicalo explicitamente en "Resumen de cambios".
