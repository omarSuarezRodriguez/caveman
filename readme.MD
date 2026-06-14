# caveman — token saver for Cursor


Uso en otros proyectos

Solo con copiar .cursor a otro proyecto ya queda listo (pero al menos hacer una vez lo de USER-RULES.global.txt , para asegurarse de que siempre se utilice el caveman, ya una vez hecho no es necesario hacer a menos que se reinstale cursor)


Copia .cursor/rules/ al repo destino
Opcional: pega USER-RULES.global.txt en Cursor → Settings → Rules → User Rules
Tokens rules siempre activos
~35 + ~45 ≈ 80 líneas vs 256 antes — anchor aislado, detail partido, sin duplicar en .cursorrules.






Based on [JuliusBrussee/caveman](https://github.com/JuliusBrussee/caveman). ~75% less output tokens. Brain big. Mouth small.

## Install in a project

1. Copy folder `.cursor/rules/` to your project root
2. (Optional) Paste `USER-RULES.global.txt` into **Cursor → Settings → Rules → User Rules**






## Files

| File | When |
|------|------|
| `caveman.mdc` | Always — loop, voice, drift recovery |
| `caveman-coding.mdc` | Always — SaaS arch, read discipline |
| `caveman-commits.mdc` | Commits |
| `caveman-review.mdc` | PR review |
| `caveman-compress.mdc` | Compress CLAUDE.md / memory files |

## Controls

- Off: `stop caveman` / `normal mode`
- Level: `caveman lite|full|ultra|wenyan`

## Why .mdc not .cursorrules

`.cursor/rules/*.mdc` with `alwaysApply: true` adheres better in Cursor. Root `.cursorrules` is only a pointer — no duplicate injection.
