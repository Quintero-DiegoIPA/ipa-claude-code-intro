# Claude Code para IPA Colombia — Guía bifurcada (mirror técnico)

> **Mirror técnico.** La versión oficial vive ahora en [juanfegarIPA/claude-code-ipa-colombia](https://github.com/juanfegarIPA/claude-code-ipa-colombia) y se publica desde **<https://juanfegaripa.github.io/claude-code-ipa-colombia/>**. Este repo se mantiene como copia funcional / espacio de experimentación bajo Diego Quintero (analyst lead). Si vas a reportar un issue o abrir un PR, prefiere el repo oficial.

Sitio Quarto con dos rutas según el tipo de trabajo: una para **Research Analysts** que escriben código (Stata, do-files, MEL), y otra para **Equipos y PMs** que delegan trabajo administrativo (comunicaciones, weekly reviews, procurement, presentaciones).

## Rutas

- **`/`** — Hub bifurcado, lleva al usuario a la ruta correcta.
- **`/analyst/`** — Para Research Analysts. Cubre VS Code + terminal, CLAUDE.md como briefing del proyecto, ejercicios prácticos de Stata.
- **`/manager/`** — Para Equipos y PMs. Cubre app de escritorio, 7 módulos por capacidad, 4 starter packs por rol, plantillas descargables.
- **`/shared/`** — Compartido y obligatorio para ambas rutas: seguridad de datos (IPA AI Usage Guidelines), bucles de feedback, prompting, recursos.
- **`/downloads/`** — Plantillas `.md` listas para descargar (CLAUDE.md, feedback.md, comunicaciones.md, etc.).

## Origen y autoría

| Ruta | Autor | Contacto |
|---|---|---|
| Manager (módulos, starter packs, plantillas) | **Juan Felipe García** — Country Director, IPA Colombia | [jfgarcia@poverty-action.org](mailto:jfgarcia@poverty-action.org) |
| Analyst (Stata, do-files, ejercicios, ejemplos) | **Diego Quintero Mogollón** — Research Analyst, IPA Colombia | [dquintero@poverty-action.org](mailto:dquintero@poverty-action.org) |
| Núcleo compartido | Co-autoría | ambos |

La fuente de verdad institucional vive en [juanfegarIPA/claude-code-ipa-colombia](https://github.com/juanfegarIPA/claude-code-ipa-colombia). Este mirror se mantiene como copia funcional bajo Diego para experimentación de la ruta analyst.

## Stack técnico

- **Quarto** + GitHub Pages (deploy automático via `quarto-actions/publish@v2`)
- **Terminal Noir** — tema dark custom con paleta IPA green (#4ea55b), tipografía DM Sans + JetBrains Mono
- **Sidebars bifurcados** activados por path (`analyst/` ve sidebar analyst, `manager/` ve sidebar manager)

## Cómo correr localmente

Requiere [Quarto](https://quarto.org/docs/get-started/) instalado.

```bash
quarto preview      # servidor de desarrollo con hot reload
quarto render       # build completo a _site/
```

## Estructura del repo

```
ipa-claude-code-intro/
├── _quarto.yml             # navbar + 2 sidebars + format html
├── styles.css              # Terminal Noir + extras (cards, buttons, grid)
├── index.qmd               # Hub bifurcado
├── README.md               # este archivo
│
├── analyst/                # Ruta A
│   ├── index.qmd, quickstart.qmd, setup.qmd, concepts.qmd,
│   ├── exercises.qmd, examples.qmd
│
├── manager/                # Ruta B
│   ├── index.qmd, empezar.qmd, instalar.qmd, plantillas.qmd
│   ├── modulos/            # 7 módulos por capacidad
│   └── starters/           # 4 starter packs por rol
│
├── shared/                 # Núcleo compartido
│   ├── safety.qmd, feedback-loops.qmd, prompting.qmd, recursos.qmd
│
├── images/                 # Gráficos SpC para examples
├── downloads/              # Plantillas .md descargables
└── .github/workflows/      # GitHub Actions de deploy
```

## Audiencia

Ambas rutas asumen familiaridad con el trabajo cotidiano en IPA y con las [IPA AI Usage Guidelines](https://ipastorage.box.com/s/mvr67ygvz1y3v8qmgjey67lk7msmyeks). La ruta analyst asume Stata avanzado; la ruta manager no asume programación.

## Contacto

Feedback de la ruta analista: [dquintero@poverty-action.org](mailto:dquintero@poverty-action.org) o [GitHub Issues de este mirror](https://github.com/Quintero-DiegoIPA/ipa-claude-code-intro/issues).

Feedback de la ruta manager o cualquier issue institucional: [jfgarcia@poverty-action.org](mailto:jfgarcia@poverty-action.org) o [GitHub Issues del repo oficial](https://github.com/juanfegarIPA/claude-code-ipa-colombia/issues).
