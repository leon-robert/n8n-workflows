# Weekly Billing Reconciliation
<a href="./weekly-billing-reconciliation-preview.png">
  <img src="./weekly-billing-reconciliation-preview.png" alt="Weekly Billing Reconciliation workflow canvas" >
</a>

**What it does**

Every Friday, this pulls the week's closed deals from a CRM </br> 
→ cross-checks them against the invoicing tool</br>
→ cross-checks them again against the project tracker</br>

Three systems that normally never talk to each other, reconciled automatically.

It catches what hides in the gaps: a deal closed with no invoice</br>
→ an invoice sent for work that was never delivered</br>
→ a client billed while their deal still shows "Open"</br>
→ numbers that don't match between systems</br>
→ duplicate records</br>
→ refunds that slipped through.

Flagged issues route straight to Slack: billing problems to one channel, delivery/data problems to another. A revenue summary writes itself into a forecast sheet, and next week's projection gets suggested automatically from the trend, with a human still deciding the final number before it's added.

**Who it's for**

Any small consultancy running its CRM, invoicing, and project tracking in separate tools that don't sync and closing out the week by hand right now.

**Stack:** Airtable (CRM) · Google Sheets (Invoicing, Forecast ! just for placeholder) · Notion (Project Tracker) · Slack (alerts + human approval)

**Setup note:** `weekly-billing-reconciliation.json` has placeholder IDs (`YOUR_..._ID`) wherever it points at a real Airtable base, Google Sheet, Notion database, Slack channel, or Slack user. Swap those for your own before importing. Credentials aren't included, obviously.
