# EUNL Yearly MSCI World Holdings (via GitHub Actions)

Dieses Repo lädt die vollständigen Holdings des iShares Core MSCI World UCITS ETF (EUNL/SWDA) und exportiert **pro Jahr ab 2010** den **spätest verfügbaren Stichtag** als CSV.

## Nutzung
1. Starte den Workflow: **Actions → EUNL Yearly Holdings → Run workflow**.
2. Ergebnisse:
   - Im Repo: `exports/eunl_yearly/`
   - Als Artifact-Download: `eunl_yearly_exports`
   - Übersicht: `summary/EUNL_yearly_summary.csv`

## Hinweise
- EUNL und SWDA sind dasselbe Fondsvehikel (ISIN IE00B4L5Y983). iShares veröffentlicht die Holdings unter SWDA; die Daten gelten für EUNL identisch.
- Kleine Lücken in sehr frühen Jahren sind möglich; der Workflow wählt pro Jahr den spätesten verfügbaren Snapshot.
