# Finance Soul Pack

> Streamline finance and accounting workflows, from journal entries and reconciliation to financial statements and variance analysis. Speed up audit prep, month-end close, and keeping your books clean.

## What It Does

- Prepare journal entries -- accruals, fixed assets, prepaids, payroll, and revenue with proper debits/credits
- Reconcile accounts -- GL-to-subledger, bank, and intercompany with reconciling item categorization
- Generate income statements with period-over-period comparison and flux analysis
- Decompose variances into drivers with narrative explanations and waterfall analysis
- Manage month-end close checklists with task sequencing and status tracking
- Generate SOX compliance testing workpapers with sample selections and control assessments

## Quick Start

### Deploy to ClawPod
[![Deploy](https://img.shields.io/badge/Deploy-ClawPod-FF6B35)](https://clawpod.app/deploy?template=finance)

### Self-host
```bash
cp -r ./* ~/.openclaw/workspace/
openclaw restart
```

Connect your ERP or data warehouse MCP servers for automated data access, or paste/upload data manually.

## Skills Included

| Skill | Description |
|-------|-------------|
| `journal-entry` | Journal entry preparation with debits/credits and supporting detail |
| `journal-entry-prep` | JE best practices, standard accrual types, documentation requirements |
| `reconciliation` | GL-to-subledger, bank, and intercompany reconciliation |
| `financial-statements` | Income statement, balance sheet, cash flow with GAAP presentation |
| `variance-analysis` | Variance decomposition (price/volume, rate/mix) with narrative and waterfall charts |
| `close-management` | Month-end close checklist, task sequencing, dependencies, status tracking |
| `sox-testing` | SOX control testing, sample selection, workpaper generation |
| `audit-support` | SOX 404 methodology, documentation standards, deficiency classification |

## Example Conversation

```
User: /journal-entry ap-accrual 2024-12
      We received services from 3 vendors in December but invoices haven't arrived yet.

Agent: Preparing AP accrual entries for December 2024:

  Entry 1 -- Vendor A (IT consulting):
    DR  6500 Professional Services    $15,000
    CR  2100 Accrued Liabilities              $15,000
    Support: SOW dated 2024-11-01, Dec services delivered per project tracker

  Entry 2 -- Vendor B (Office maintenance):
    DR  6200 Facilities Expense       $3,200
    CR  2100 Accrued Liabilities              $3,200
    Support: Monthly contract at $3,200/mo

  [Continues for all vendors with full supporting detail]
  Total accrual: $23,700 | Reversal: Auto-reverse 2025-01-01
```

## Origin

Adapted from Anthropic's Knowledge Work Plugins (`finance` plugin v1.2.0).
