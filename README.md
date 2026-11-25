# Wuolah Campaign Analysis — Claude Code Skill

Skill de Claude Code para analizar campañas de publicidad en Wuolah. Extrae datos de la API de WuolAds, compara con benchmarks de la plataforma y genera informes completos con insights accionables.

## Qué hace

- Analiza campañas a nivel de campaña, ad set y creativo
- Compara rendimiento vs benchmarks reales de la plataforma
- Calcula el valor diferencial de Apuntes (Time-In-View de 76 min/doc)
- Analiza post-campaign clicks (long tail de PDFs)
- Segmentación geotemporal (ciudades, horas, días)
- Genera informes con cumplimiento de objetivos (YTD)

## Requisitos

- [Claude Code](https://docs.anthropic.com/en/docs/claude-code) instalado
- MCP server de **WuolAds** configurado en tu Claude Code

## Instalación

Copia la carpeta de la skill a tu directorio de skills de Claude Code:

```bash
# Clona el repo
git clone https://github.com/wuolah-free/wuolah-campaign-analysis.git

# Copia la skill
cp -r wuolah-campaign-analysis ~/.claude/skills/wuolah-campaign-analysis
```

Listo. La próxima vez que abras Claude Code, la skill estará disponible.

## Uso

Simplemente pide un análisis de campaña en Claude Code:

```
Analiza la campaña del anunciante 12345
```

```
¿Cómo va la campaña de [cliente]?
```

```
Dame un informe de campaña de [marca]
```

La skill se activa automáticamente cuando detecta que quieres analizar rendimiento publicitario en Wuolah.

## Estructura

```
wuolah-campaign-analysis/
├── SKILL.md              # Skill principal
├── README.md             # Este archivo
└── references/
    └── formatos-specs.md # Specs de todos los formatos de Wuolah
```

## Licencia

Uso interno Wuolah.
