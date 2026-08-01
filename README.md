## n8n-workflows

Production-ready n8n automation workflows — built, tested, documented.

What this is

A working library of automation workflows I've built with n8n. Each one solves a specific operational problem for a business — not a proof-of-concept, a workflow that runs.

How this repo is organized
n8n-workflows/
├── portfolio/          # Workflows built to showcase capability
├── client-templates/   # Reusable, adaptable workflows for new engagements
├── internal/           # Personal tooling and internal automations
├── monitoring/         # Workflows that watch systems and alert on issues
└── README.md
How each workflow is documented

Every entry below follows the same structure, so anyone can scan it fast:

Problem — what was broken or manual before this existed
Solution — what the workflow does, step by step
Stack — services/APIs connected
Result — the measurable outcome (time saved, errors reduced, volume handled)
Workflows
Portfolio
secure-lead-intake-webhook
Problem: Leads submitted through a web form required manual entry into [CRM], delaying first response by [X hours/minutes].
Solution: Webhook captures form submissions and routes them automatically to [CRM / email / Slack — name the real target].
Stack: Webhook, [service 1], [service 2]
Result: [X]% faster response time, or [X] minutes saved per lead.
<!-- Copy the block above for each new workflow. Keep the same four fields, always in this order. -->
Client Templates

(in progress)

Internal

(in progress)

Monitoring

(in progress)

Security

No credentials, API keys, or tokens are stored in this repository. All workflows reference sensitive values through environment variables, never hardcoded.

Contact

Robert Leon — [email or LinkedIn link] Building automation systems that stop SMB owners from being the bottleneck in their own business.
