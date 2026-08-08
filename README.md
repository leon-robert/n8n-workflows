<h1>n8n-workflows</h1>

Automation workflows I've built with n8n, a mix of self-initiated projects and generalized client work. Each one is documented the same way: what it does, who it's for, the problem it solves.

<h3>Structure</h3>

<pre>
n8n-workflows/
├── portfolio/
│   └── [workflow-name]/     — workflow.json + its own README
├── internal/
│   └── [workflow-name]/     — my own tooling, not client-facing
├── monitoring/
│   └── [workflow-name]/     — watches systems, alerts on issues
└── README.md
</pre>

<h3>Portfolio Workflows</h3>

| Workflow | What it does |
|---|---|
| [freelancer-lead-intake-system](portfolio/freelancer-lead-intake-system/) | Captures inbound leads, scores and qualifies them, and logs qualified leads to Airtable with a Slack alert, no manual follow-up tracking. |
| [ai-customer-support-triage](portfolio/ai-customer-support-triage/) | Reads incoming support tickets, classifies and prioritizes them with AI, and routes each to the right queue, no manual sorting. |
| [ai-business-assistant-for-professional-services](portfolio/ai-business-assistant-for-professional-services/) | Handles routine client requests with AI, flags anything below a confidence threshold for human review, and logs every decision to an audit trail. |
| [freelancerOS](portfolio/freelancerOS/) | Routes call bookings, lead tracking, and time logs through one system, with alerts for anything it doesn't recognize. |
| [weekly-billing-reconciliation](./portfolio/weekly-billing-reconciliation) | Reconciles CRM, invoicing, and project data every Friday and flags what doesn't add up, no manual cross-checking. |

<h3>Security</h3>

No credentials, API keys, or tokens are stored in this repository. Every workflow references sensitive values through environment variables, never hardcoded. Workflows derived from client work are generalized. Company-specific details and some nodes are changed to protect confidentiality.

<h3>Get in touch</h3>

[your website] · [your email] · [your LinkedIn]
