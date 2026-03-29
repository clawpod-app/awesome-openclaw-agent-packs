[English](./README.md) | [中文](./README.zh-CN.md) | [日本語](./README.ja.md) | [Español](./README.es.md) | [Deutsch](./README.de.md)

# Awesome OpenClaw Agent Packs

**Packs de agentes IA preconfigurados para OpenClaw. Elige un rol, despliega en Telegram y empieza a trabajar.**

[![Desplegar en ClawPod](https://img.shields.io/badge/Desplegar%20en-ClawPod-FF6B35?style=for-the-badge)](https://clawpod.app/templates)
![Packs](https://img.shields.io/badge/Packs-11-blue?style=for-the-badge)
![Habilidades](https://img.shields.io/badge/Habilidades-92-purple?style=for-the-badge)
![Licencia](https://img.shields.io/badge/Licencia-MIT-green?style=for-the-badge)

---

## ¿Qué es esto?

Cada pack convierte un agente OpenClaw genérico en un miembro especializado del equipo. Un **Copiloto de Ventas** que prepara llamadas, investiga prospectos y redacta mensajes de seguimiento. Un **Copiloto de Ingeniería** que hace standups, revisiones de código y respuesta a incidentes. Un **Analista Legal** que revisa contratos y verifica el cumplimiento normativo.

Cada pack incluye 6 archivos de definición + un directorio completo de `skills/`:

```
packs/sales/
├── SOUL.md          # Quién es el agente (personalidad, valores, estilo de comunicación)
├── AGENTS.md        # Comportamiento al iniciar, habilidades disponibles, flujos de trabajo
├── HEARTBEAT.md     # Tareas programadas (briefings diarios, revisiones semanales)
├── TOOLS.md         # Herramientas conectadas y configuración MCP
├── MEMORY.md        # Cómo el agente recuerda contexto entre sesiones
├── README.md        # Guía de configuración
└── skills/          # 9 flujos de trabajo
    ├── account-research/    → Investigar cualquier empresa o prospecto
    ├── call-prep/           → Preparar llamadas de ventas con contexto
    ├── draft-outreach/      → Emails y mensajes de LinkedIn personalizados
    ├── pipeline-review/     → Analizar salud de deals y detectar riesgos
    ├── forecast/            → Proyecciones de ingresos ponderadas
    └── ...                  → + 4 más
```

---

## Packs Disponibles

| Pack | Habilidades | Dominio | Desplegar |
|------|-------------|---------|-----------|
| [Copiloto de Ventas](./packs/sales/) | 9 | Ventas e Ingresos | [![Desplegar](https://img.shields.io/badge/Desplegar-ClawPod-FF6B35)](https://clawpod.app/templates/sales) |
| [Copiloto de Ingeniería](./packs/engineering/) | 10 | Ingeniería de Software | [![Desplegar](https://img.shields.io/badge/Desplegar-ClawPod-FF6B35)](https://clawpod.app/templates/engineering) |
| [Analista de Datos](./packs/data/) | 10 | Datos y Analítica | [![Desplegar](https://img.shields.io/badge/Desplegar-ClawPod-FF6B35)](https://clawpod.app/templates/data) |
| [Estratega de Marketing](./packs/marketing/) | 8 | Marketing y Contenido | [![Desplegar](https://img.shields.io/badge/Desplegar-ClawPod-FF6B35)](https://clawpod.app/templates/marketing) |
| [Analista Legal](./packs/legal/) | 9 | Legal y Cumplimiento | [![Desplegar](https://img.shields.io/badge/Desplegar-ClawPod-FF6B35)](https://clawpod.app/templates/legal) |
| [Analista Financiero](./packs/finance/) | 8 | Finanzas y Contabilidad | [![Desplegar](https://img.shields.io/badge/Desplegar-ClawPod-FF6B35)](https://clawpod.app/templates/finance) |
| [Product Manager](./packs/product-management/) | 8 | Gestión de Producto | [![Desplegar](https://img.shields.io/badge/Desplegar-ClawPod-FF6B35)](https://clawpod.app/templates/product-management) |
| [Partner de RRHH](./packs/human-resources/) | 9 | RRHH y Personal | [![Desplegar](https://img.shields.io/badge/Desplegar-ClawPod-FF6B35)](https://clawpod.app/templates/human-resources) |
| [Soporte al Cliente](./packs/customer-support/) | 5 | Atención al Cliente | [![Desplegar](https://img.shields.io/badge/Desplegar-ClawPod-FF6B35)](https://clawpod.app/templates/customer-support) |
| [Partner de Diseño](./packs/design/) | 7 | UX y Diseño | [![Desplegar](https://img.shields.io/badge/Desplegar-ClawPod-FF6B35)](https://clawpod.app/templates/design) |
| [Gerente de Operaciones](./packs/operations/) | 9 | Operaciones | [![Desplegar](https://img.shields.io/badge/Desplegar-ClawPod-FF6B35)](https://clawpod.app/templates/operations) |

---

## Inicio Rápido

### Opción A: Despliegue con un clic (recomendado)

1. Elige un pack de la tabla y haz clic en **Desplegar en ClawPod**
2. Ingresa tu token de Telegram Bot
3. Tu agente estará activo en 30 segundos en [clawpod.app](https://clawpod.app)

Sin Docker, sin VPS, sin archivos de configuración.

### Opción B: Autoalojamiento con OpenClaw

```bash
git clone https://github.com/clawpod-app/awesome-openclaw-agent-packs.git
cp -r awesome-openclaw-agent-packs/packs/sales/* ~/.openclaw/workspace/
openclaw gateway restart
```

Tu agente lee `SOUL.md` al iniciar, carga las habilidades de `skills/` y comienza a trabajar.

### Opción C: Configuración manual

1. Copia cualquier pack al directorio workspace de OpenClaw
2. Configura las API keys y herramientas MCP según `TOOLS.md`
3. Reinicia tu agente

---

## Cómo Funcionan las Habilidades

Las habilidades son guías de flujo de trabajo basadas en texto, no scripts ejecutables. Cuando un usuario pregunta "investiga Acme Corp", el agente:

1. Lee `skills/account-research/SKILL.md`
2. Sigue el flujo de trabajo paso a paso definido dentro
3. Usa las herramientas disponibles (búsqueda web, conectores MCP) para ejecutar
4. Devuelve un resultado estructurado

Las habilidades funcionan de forma independiente con búsqueda web. Mejoran al conectar herramientas MCP (CRM, email, calendario), pero son completamente funcionales sin ellas.

---

## Contribuir

¡Damos la bienvenida a nuevos packs! Requisitos:

1. Los 6 archivos principales: `SOUL.md`, `AGENTS.md`, `HEARTBEAT.md`, `TOOLS.md`, `MEMORY.md`, `README.md`
2. Al menos una habilidad con un flujo `SKILL.md` completo
3. Probado en una instancia real de OpenClaw o ClawPod
4. README con pasos de configuración y conversaciones de ejemplo

Consulta cualquier pack existente para ver el formato esperado.

---

## Atribución

Adaptado de [Knowledge Work Plugins de Anthropic](https://github.com/anthropics/knowledge-work-plugins) (Apache-2.0). Ver [NOTICE](./NOTICE) para detalles.

## Licencia

MIT. Las habilidades de Knowledge Work derivan del trabajo con licencia Apache-2.0 de Anthropic. Ver [LICENSE](./LICENSE).

---

*Mantenido por [ClawPod](https://clawpod.app) — Despliega tu bot de IA en Telegram en 30 segundos.*
