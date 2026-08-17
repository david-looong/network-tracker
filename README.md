# network-tracker

Data store for the "Network Tracker" Claude Code subagent and its daily
report routine.

## contacts.csv

Columns:

- `name` — contact's full name
- `role` — their role / title (and company, if not your own)
- `last_contacted` — date you last reached out, `YYYY-MM-DD`

Update `last_contacted` whenever you message, email, or meet with someone.
Add new rows for new contacts.

## Report thresholds

- **14–29 days** since last contact → "consider reaching out" nudge
- **30+ days** since last contact → "strongly reach out" nudge
