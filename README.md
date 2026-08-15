# Experto global en emergencias tecnológicas, CBRN e infraestructura crítica

Sistema mixto para Claude: skill + catálogo + investigación en vivo. El catálogo dice a quién preguntar. Las fuentes oficiales del día dan el dato.

Cubre accidente químico, radiológico, nuclear, industrial, presa, relaves, apagón e infraestructura crítica. No sustituye al experto en desastres naturales, al de salud pública ni al de voluntarios.

El skill vive en `.claude/skills/`, no en `.cursor/skills/`.

## Claude Code (uso principal)

1. Clona el repo y abre Claude Code **dentro de esta carpeta**.
2. Claude carga `CLAUDE.md` y descubre el skill `.claude/skills/experto-cbrn-tecnologico/`.
3. Pregunta en el chat, o invoca `/experto-cbrn-tecnologico`.

Ejemplos:

- Sitrep de un accidente industrial en [país].
- Perfil de regulador nuclear / químico / de presas de Japón / Nigeria / Brasil.
- ¿Hay notificación IAEA o nivel INES publicado?
- Quién manda un derrame en Nigeria (NOSDRA, no EPA).
- Cruce: sismo + refinería, o tsunami + planta nuclear.

Guía completa: [USO-CLAUDE.md](USO-CLAUDE.md).

## Qué hay aquí

| Capa | Ruta |
| --- | --- |
| Identidad (Claude Code) | [CLAUDE.md](CLAUDE.md) |
| Skill | [.claude/skills/experto-cbrn-tecnologico/SKILL.md](.claude/skills/experto-cbrn-tecnologico/SKILL.md) |
| Taxonomía y familias | [knowledge/taxonomy/](knowledge/taxonomy/), [knowledge/families/](knowledge/families/) |
| Sistemas, derecho, personas | [knowledge/systems/](knowledge/systems/), [knowledge/legal/](knowledge/legal/), [knowledge/personas/](knowledge/personas/) |
| Marcos (IAEA, OPCW, TEIA, presas) | [knowledge/frameworks/index.md](knowledge/frameworks/index.md) |
| Sitios y casos | [knowledge/sites/](knowledge/sites/), [knowledge/cases/](knowledge/cases/) |
| Organismos | [knowledge/organizations/index.md](knowledge/organizations/index.md) |
| Plataformas | [knowledge/platforms/index.md](knowledge/platforms/index.md) |
| Países y anclas | [knowledge/countries/_index.md](knowledge/countries/_index.md) |
| Playbooks | [playbooks/](playbooks/) |
| Mapa de expertos hermanos | [knowledge/research/mapa-expertos-hermanos.md](knowledge/research/mapa-expertos-hermanos.md) |

## Reglas

- Cobertura mundial. Nunca default a una sola región.
- Nombres oficiales de reguladores en el idioma local.
- Citar fuentes. No inventar INES, notificaciones ni roturas.
- Español latino neutro en la respuesta. Documentos en su idioma original.

## Límites

Los nombres de reguladores y las URL cambian. Verificar el sitio nacional y el de IAEA u OPCW. Este proyecto no reemplaza a EXPERTO DESASTRES NATURALES, EXPERTO SALUD PUBLICA ni EXPERTO VOLUNTARIOS.
