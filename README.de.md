[English](./README.md) | [中文](./README.zh-CN.md) | [日本語](./README.ja.md) | [Español](./README.es.md) | [Deutsch](./README.de.md)

# Awesome OpenClaw Agent Packs

**Vorkonfigurierte KI-Agenten-Pakete für OpenClaw. Rolle wählen, auf Telegram deployen, sofort loslegen.**

[![Auf ClawPod deployen](https://img.shields.io/badge/Deployen%20auf-ClawPod-FF6B35?style=for-the-badge)](https://clawpod.app/templates)
![Pakete](https://img.shields.io/badge/Pakete-11-blue?style=for-the-badge)
![Skills](https://img.shields.io/badge/Skills-92-purple?style=for-the-badge)
![Lizenz](https://img.shields.io/badge/Lizenz-MIT-green?style=for-the-badge)

---

## Was ist das?

Jedes Paket verwandelt einen generischen OpenClaw-Agenten in ein spezialisiertes Teammitglied. Ein **Sales Co-Pilot**, der Anrufe vorbereitet, Interessenten recherchiert und Outreach-Nachrichten verfasst. Ein **Engineering Co-Pilot**, der Standups, Code-Reviews und Incident Response durchführt. Ein **Legal Analyst**, der Verträge prüft und Compliance überprüft.

Jedes Paket enthält 6 Definitionsdateien + ein vollständiges `skills/`-Verzeichnis:

```
packs/sales/
├── SOUL.md          # Wer der Agent ist (Persönlichkeit, Werte, Kommunikationsstil)
├── AGENTS.md        # Startverhalten, verfügbare Skills, Workflows
├── HEARTBEAT.md     # Geplante Aufgaben (tägliche Briefings, wöchentliche Pipeline-Reviews)
├── TOOLS.md         # Verbundene Tools und MCP-Konfiguration
├── MEMORY.md        # Wie der Agent Kontext über Sitzungen hinweg speichert
├── README.md        # Einrichtungsanleitung
└── skills/          # 9 Skill-Workflows
    ├── account-research/    → Unternehmen oder Interessenten recherchieren
    ├── call-prep/           → Verkaufsgespräche mit Kontext vorbereiten
    ├── draft-outreach/      → Personalisierte E-Mails und LinkedIn-Nachrichten
    ├── pipeline-review/     → Deal-Gesundheit analysieren und Risiken erkennen
    ├── forecast/            → Gewichtete Umsatzprognosen
    └── ...                  → + 4 weitere
```

---

## Verfügbare Pakete

| Paket | Skills | Bereich | Deployen |
|-------|--------|---------|----------|
| [Sales Co-Pilot](./packs/sales/) | 9 | Vertrieb & Umsatz | [![Deployen](https://img.shields.io/badge/Deployen-ClawPod-FF6B35)](https://clawpod.app/templates/sales) |
| [Engineering Co-Pilot](./packs/engineering/) | 10 | Softwareentwicklung | [![Deployen](https://img.shields.io/badge/Deployen-ClawPod-FF6B35)](https://clawpod.app/templates/engineering) |
| [Datenanalyst](./packs/data/) | 10 | Daten & Analytik | [![Deployen](https://img.shields.io/badge/Deployen-ClawPod-FF6B35)](https://clawpod.app/templates/data) |
| [Marketing-Stratege](./packs/marketing/) | 8 | Marketing & Content | [![Deployen](https://img.shields.io/badge/Deployen-ClawPod-FF6B35)](https://clawpod.app/templates/marketing) |
| [Legal Analyst](./packs/legal/) | 9 | Recht & Compliance | [![Deployen](https://img.shields.io/badge/Deployen-ClawPod-FF6B35)](https://clawpod.app/templates/legal) |
| [Finanzanalyst](./packs/finance/) | 8 | Finanzen & Buchhaltung | [![Deployen](https://img.shields.io/badge/Deployen-ClawPod-FF6B35)](https://clawpod.app/templates/finance) |
| [Product Manager](./packs/product-management/) | 8 | Produktmanagement | [![Deployen](https://img.shields.io/badge/Deployen-ClawPod-FF6B35)](https://clawpod.app/templates/product-management) |
| [HR-Partner](./packs/human-resources/) | 9 | HR & Personal | [![Deployen](https://img.shields.io/badge/Deployen-ClawPod-FF6B35)](https://clawpod.app/templates/human-resources) |
| [Kundensupport](./packs/customer-support/) | 5 | Kundenservice | [![Deployen](https://img.shields.io/badge/Deployen-ClawPod-FF6B35)](https://clawpod.app/templates/customer-support) |
| [Design-Partner](./packs/design/) | 7 | UX & Design | [![Deployen](https://img.shields.io/badge/Deployen-ClawPod-FF6B35)](https://clawpod.app/templates/design) |
| [Operations Manager](./packs/operations/) | 9 | Geschäftsbetrieb | [![Deployen](https://img.shields.io/badge/Deployen-ClawPod-FF6B35)](https://clawpod.app/templates/operations) |

---

## Schnellstart

### Option A: One-Click Deploy (empfohlen)

1. Wähle ein Paket aus der Tabelle und klicke auf **Auf ClawPod deployen**
2. Gib deinen Telegram Bot Token ein
3. Dein Agent ist in 30 Sekunden live auf [clawpod.app](https://clawpod.app)

Kein Docker, kein VPS, keine Konfigurationsdateien.

### Option B: Self-Hosting mit OpenClaw

```bash
git clone https://github.com/clawpod-app/awesome-openclaw-agent-packs.git
cp -r awesome-openclaw-agent-packs/packs/sales/* ~/.openclaw/workspace/
openclaw gateway restart
```

Dein Agent liest `SOUL.md` beim Start, lädt die Skills aus `skills/` und beginnt sofort zu arbeiten.

### Option C: Manuelle Einrichtung

1. Kopiere ein beliebiges Paket in dein OpenClaw Workspace-Verzeichnis
2. Konfiguriere API-Schlüssel und MCP-Tools gemäß `TOOLS.md`
3. Starte deinen Agenten neu

---

## Wie Skills funktionieren

Skills sind textbasierte Workflow-Anleitungen, keine ausführbaren Skripte. Wenn ein Benutzer fragt „Recherchiere Acme Corp", dann:

1. Liest der Agent `skills/account-research/SKILL.md`
2. Folgt dem schrittweisen Workflow darin
3. Nutzt verfügbare Tools (Websuche, MCP-Konnektoren) zur Ausführung
4. Liefert strukturierte Ergebnisse

Skills funktionieren eigenständig mit Websuche. Sie werden besser mit MCP-Tools (CRM, E-Mail, Kalender), sind aber auch ohne diese voll funktionsfähig.

---

## Beitragen

Wir freuen uns über neue Pakete! Anforderungen:

1. Alle 6 Kerndateien: `SOUL.md`, `AGENTS.md`, `HEARTBEAT.md`, `TOOLS.md`, `MEMORY.md`, `README.md`
2. Mindestens ein Skill mit vollständigem `SKILL.md`-Workflow
3. Getestet auf einer echten OpenClaw- oder ClawPod-Instanz
4. README mit Einrichtungsschritten und Beispielkonversationen

Orientiere dich am Format der bestehenden Pakete.

---

## Namensnennung

Adaptiert von [Anthropics Knowledge Work Plugins](https://github.com/anthropics/knowledge-work-plugins) (Apache-2.0). Siehe [NOTICE](./NOTICE) für Details.

## Lizenz

MIT. Knowledge Work Skills basieren auf Anthropics Apache-2.0-lizenziertem Werk. Siehe [LICENSE](./LICENSE).

---

*Gepflegt von [ClawPod](https://clawpod.app) — Deploye deinen KI-Telegram-Bot in 30 Sekunden.*
