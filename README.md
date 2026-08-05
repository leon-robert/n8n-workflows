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

<h3>Workflows</h3>

| Workflow | What it does |
|---|---|
| [secure-lead-intake-webhook](portfolio/secure-lead-intake-webhook/) | Captures form submissions and routes them automatically, no manual entry. |
| [weekly-billing-reconciliation](./portfolio/weekly-billing-reconciliation) | Reconciles CRM, invoicing, and project data every Friday and flags what doesn't add up, no manual cross-checking. |

<h3>Security</h3>

No credentials, API keys, or tokens are stored in this repository. Every workflow references sensitive values through environment variables, never hardcoded. Workflows derived from client work are generalized. Company-specific details and some nodes are changed to protect confidentiality.

<h3>Get in touch</h3>

[your website] · [your email] · [your LinkedIn]
