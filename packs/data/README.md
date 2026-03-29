# Data Soul Pack

> Write SQL, explore datasets, and generate insights faster. Build visualizations and dashboards, and turn raw data into clear stories for stakeholders.

## What It Does

- Answer data questions end-to-end -- from SQL to insight to visualization
- Profile and explore datasets to understand shape, quality, and patterns
- Write optimized SQL for any dialect (Snowflake, BigQuery, Databricks, PostgreSQL, etc.)
- Create publication-quality visualizations with Python
- Build interactive HTML dashboards with Chart.js, filters, and styling
- Validate analyses for methodology, accuracy, and bias before sharing
- Extract schema context from connected data sources for better query generation

## Quick Start

### Deploy to ClawPod
[![Deploy](https://img.shields.io/badge/Deploy-ClawPod-FF6B35)](https://clawpod.app/deploy?template=data)

### Self-host
```bash
cp -r ./* ~/.openclaw/workspace/
openclaw restart
```

Connect your data warehouse MCP server for direct query execution, or paste results / upload CSV files.

## Skills Included

| Skill | Description |
|-------|-------------|
| `analyze` | Answer data questions from quick lookups to full analyses |
| `explore-data` | Profile datasets -- shape, quality, distributions, patterns |
| `write-query` | Write optimized SQL for any dialect with best practices |
| `create-viz` | Publication-quality Python visualizations |
| `build-dashboard` | Interactive HTML dashboards with Chart.js and filters |
| `validate-data` | Pre-delivery QA -- methodology, accuracy, bias checks |
| `sql-queries` | SQL best practices, common patterns, performance optimization |
| `data-visualization` | Chart selection guide, Python viz patterns, design principles |
| `statistical-analysis` | Descriptive stats, trend analysis, outlier detection, hypothesis testing |
| `data-context-extractor` | Extract schema context from connected data sources |

## Example Conversation

```
User: /analyze What was our monthly revenue trend for the past 12 months,
      broken down by product line?

Agent: [Writes SQL query against your data warehouse]
       [Executes and retrieves results]
       [Generates trend line chart]

       Key findings:
       - Product line A grew 23% YoY, accelerating in Q4
       - Product line B was flat (+1.2%), seasonal pattern consistent with prior year
       - Product line C is new (launched in July) and already 8% of total revenue

       [Sanity check: total matches the GL revenue figure within 0.3%]
       Want me to dig deeper into any product line?
```

## Origin

Adapted from Anthropic's Knowledge Work Plugins (`data` plugin v1.1.0).
