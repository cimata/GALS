# GA Fact-Check Desk para Claude

Adaptación a Claude del plugin «GA Fact-Check Desk» exportado desde ChatGPT. Contiene un skill (`fact-check`) con la metodología y el formato de salida de referencia, y un comando `/fact-check`.

## Estructura

```
ga-fact-check-desk/
├── .claude-plugin/plugin.json      manifiesto del plugin
├── commands/fact-check.md          comando /fact-check
├── skills/fact-check/
│   ├── SKILL.md                    instrucciones del GPT + flujo de trabajo
│   └── references/
│       ├── methodology.md          metodología v2 (sin cambios)
│       └── output-format.md        formato de salida v2 (sin cambios)
└── assets/icon.png                 icono original (Claude Code no lo usa)
```

## Instalación

Claude Code: `/plugin marketplace add cimata/gals` y después `/plugin install ga-fact-check-desk@gals`. En local también vale `claude --plugin-dir plugins/ga-fact-check-desk`.

Claude.ai / Claude Desktop / Cowork: sube `dist/ga-fact-check-desk-skill.zip` en Ajustes → Capacidades → Skills. Si ya existe un skill con el mismo nombre, sustitúyelo.

## Cambios respecto al original de ChatGPT

- Se eliminan `extensions.com.openai`, `agents/openai.yaml` y `lookup/knowledge-index.json`, que solo tienen sentido en ChatGPT.
- Las referencias a «archivos de Knowledge» pasan a apuntar a `references/`.
- Se elimina el ZIP anidado `GA_Fact_Check_Desk_skill_v2.zip`; su metodología y formato eran idénticos a los dos `.md`, y su flujo de trabajo y reglas no negociables se han integrado en `SKILL.md`.
- Se añade un apartado de herramientas (WebSearch/WebFetch y qué hacer sin acceso web).
- Se resuelve la discrepancia de etiquetas entre las instrucciones («REVISIÓN HUMANA») y el formato («REQUIERE JUICIO HUMANO») a favor de las instrucciones, que en el original tenían prioridad.
