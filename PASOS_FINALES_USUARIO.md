# PASOS FINALES (SOLO ESTO TIENES QUE HACER)

1. **Validar en navegador y tomar capturas**
- Abre cada archivo en `original/` y `corregido/`.
- Ejecuta: WAVE + Axe + Lighthouse (minimo 3 herramientas).
- Guarda capturas en `evidencias/screenshots/` con nombres before/after.

2. **Completar resultados**
- Abre `validacion/proceso-validacion.md`.
- Rellena la tabla "Antes/Despues" con los resultados reales.

3. **(Opcional) Prueba comparativa de asistentes**
- Si quieres comparar Copilot vs Gemini, completa `validacion/ejecucion-asistentes.md`.

4. **Subir a GitHub**
```bash
git add .
git commit -m "docs: evidencias finales de validacion"
gh repo create accesibilidad-wcag-prompt --public --source . --remote origin --push
```

5. **Entregar enlace del repo**
- Comparte la URL del repositorio y confirma que incluye:
  - `original/` y `corregido/`
  - `prompts/prompt-perfecto.md`
  - `README.md`
  - `validacion/*.md`
  - `evidencias/screenshots/*`
