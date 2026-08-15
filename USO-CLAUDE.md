# Cómo usar este experto en Claude

El catálogo (`knowledge/`, `playbooks/`) no cambia. Cambia el envoltorio: Claude Code lee `CLAUDE.md` y el skill en `.claude/skills/`. claude.ai usa un Project con instrucciones y archivos subidos.

## 1. Claude Code (recomendado)

1. Abre Claude Code **dentro de esta carpeta**.
2. Pregunta o usa `/experto-cbrn-tecnologico`.

Claude debe:

- Leer `.claude/skills/experto-cbrn-tecnologico/SKILL.md`
- Abrir la ficha de país en `knowledge/countries/`
- Aplicar el playbook
- Buscar en la web en el idioma oficial (regulador nuclear, autoridad química, presas, ambiente)

Si el skill no dispara solo, invócalo con `/experto-cbrn-tecnologico`.

Skill personal (todos tus proyectos): copia `.claude/skills/experto-cbrn-tecnologico/` a `%USERPROFILE%\.claude\skills\` (Windows) o `~/.claude/skills/` (macOS/Linux). El catálogo completo solo existe si también tienes este repo abierto.

## 2. claude.ai: Project

1. Crea un Project en claude.ai.
2. Instrucciones del Project: pega el contenido de `CLAUDE.md`.
3. Sube archivos de conocimiento, en este orden si hay límite de tamaño:

**Obligatorios**

- `CLAUDE.md`
- `.claude/skills/experto-cbrn-tecnologico/SKILL.md`
- `playbooks/` (todos)
- `knowledge/taxonomy/`
- `knowledge/frameworks/`
- `knowledge/organizations/`
- `knowledge/platforms/`
- `knowledge/research/protocolo-multilenguaje.md`
- `knowledge/countries/_index.md`
- `knowledge/countries/iso-index.md`
- `knowledge/countries/_schema.md`
- `knowledge/countries/anclas.md`
- `knowledge/families/`
- `knowledge/systems/`
- `knowledge/sites/_index.md`
- `knowledge/cases/index.md`

**Países (el mapa mundial)**

- `knowledge/countries/africa.md`
- `knowledge/countries/americas.md`
- `knowledge/countries/asia.md`
- `knowledge/countries/europe.md`
- `knowledge/countries/oceania.md`
- `knowledge/countries/territories.md`

4. Activa búsqueda web en el Project si el producto lo permite. Sin web, Claude solo usa el catálogo (nombres y rutas), no datos del día.

## 3. Subir solo el skill (ajustes de Claude / API)

La carpeta `.claude/skills/experto-cbrn-tecnologico/` es un Agent Skill (`SKILL.md` + `references/`).

Sirve para las reglas. No metas todo `knowledge/` dentro de `SKILL.md`.

## 4. Comprobar que está bien adaptado

Pide estas consultas. El enrutamiento correcto está en `playbooks/casos-validacion.md`.

1. Accidente nuclear en Japón → 原子力規制委員会. No NRC.
2. Accidente industrial en Indonesia → BAPETEN + KLH. No PAHO ni Seveso como ley local.
3. Derrame en Nigeria → NOSDRA. No EPA.
4. Relaves en Brasil → ANM + IBAMA + CNEN si hay radioactividad. No copiar NRC.
5. Presa en India → Central Water Commission / autoridad estatal. No IAEA.
6. Francia → ASNR (verificar nombre vigente). No FEMA.
7. Ucrania nuclear → Держатомрегулювання + IAEA. Declarar límite de conflicto.
8. Vanuatu / SIDS → autoridad nacional. No copiar Seveso.
9. Sismo + refinería → cruce a EXPERTO DESASTRES NATURALES.
10. Heridos por nube tóxica → cruce a EXPERTO SALUD PUBLICA. No recetar.
11. Fuente huérfana → regulador radiológico, no sitrep de reactor.
12. Relaves Brumadinho → ANM, no IAEA.
13. Donar yodo o trajes → lista del Estado o no enviar.
14. Lagos → ficha de sitio + NOSDRA federal. No fusionar.

Si alguna respuesta defaulta a NRC, EPA, FEMA o Seveso fuera de su ámbito, el skill no se aplicó.

## Qué no cambia

- `knowledge/` y `playbooks/` son la misma fuente de verdad.
- El flujo sigue siendo: clasificar evento y familia → IAEA/OPCW/TEIA/presa → región → país → sitio si aplica → idioma local → fuentes vivas.
