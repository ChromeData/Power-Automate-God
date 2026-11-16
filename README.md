# Power Automate God

Production Power Automate flows I designed, built and support for a nonprofit, replacing hours of manual data entry, document prep and follow-up each week.

## Highlights

- **Idempotent by design.** Logs and dedupe checks before every write, so reruns never double-send or double-copy.
- **Human-in-the-loop.** Anything external stops at a draft for review.
- **Maintainable.** Parameterized settings, self-documenting step names, single-alert error handling.
- **Safe testing.** Test modes run against live data without reaching real recipients.

## Automations

| # | Automation | Summary | Schedule |
|---|---|---|---|
| 01 | [Daily donation receipts](automations/01-daily-donation-receipts.md) | Generates receipt PDFs and ready-to-send email drafts for new gifts | Daily |
| 02 | [Signed forms → master database](automations/02-signed-forms-to-master-database.md) | Syncs completed e-signature forms and attachments | Every 15 min |
| 03 | [CRM contracts → master database](automations/03-crm-contracts-to-master-database.md) | Syncs new contracts with their current PDF | Hourly |
| 04 | [Contractor pay engine](automations/04-contractor-pay-engine.md) | Reconciles contractor paperwork and files documents | Every 15 min |
| 05 | [Weekly giving digest](automations/05-weekly-giving-digest.md) | Builds and shares the weekly gifts report | Weekly |

## Security note

Flow exports, screenshots, product names and real data are intentionally withheld. They expose internal IDs, system connections and the organization's tech stack. The write-ups cover the architecture and logic only.
