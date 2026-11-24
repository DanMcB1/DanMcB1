# Daniel McBrearty

**Forward Deployed Engineer / Solutions Engineer**

I come from car sales, F&I, and auto software sales (most recently at [Dealr.cloud](https://dealr.cloud)). That background is the point: I know how dealerships work, how customers talk about risk, and what has to be true before anyone will let an AI near a live system. I built the 12 working demos below with AI-assisted coding to show how I would approach the problems a Forward Deployed or solutions engineer hits on a real engagement.

They are **portfolio demos** with sample data for a fictional dealer group, Lakeside Auto Group — not production systems, and not a claim of years of software-engineering experience. Each repo has a README, a one-minute demo script, and tests, and each one runs locally with no paid cloud required.

## Business value

| Project | What it does | Tech |
| --- | --- | --- |
| [Architecture Scoper](https://github.com/DanMcB1/ai-architecture-scoper) | Turns a vague “we want AI” request into a 4-week statement of work. | Python, Streamlit, rules engine |
| [FinOps ROI Dashboard](https://github.com/DanMcB1/ai-finops-roi-dashboard) | Shows AI cost and time saved by department, from sample usage data. | Python, Streamlit, Pandas, Plotly |
| [Shadow Replay Harness](https://github.com/DanMcB1/ai-shadow-replay) | Replays past tickets through a candidate AI agent and issues a go / no-go before anything reaches a customer. | Python, Streamlit, Pandas, Plotly |
| [Customer Admin Portal](https://github.com/DanMcB1/ai-customer-admin-portal) | Lets a customer’s IT admin edit, test, publish, and roll back an AI assistant’s script — and keeps one dealership from seeing another’s data. | Python, FastAPI, Streamlit, SQLite, SQLModel |

## Security and trust

| Project | What it does | Tech |
| --- | --- | --- |
| [SSO Agent Delegation Broker](https://github.com/DanMcB1/ai-sso-agent-broker) | An employee signs in with SSO and lends an AI agent a five-minute, limited-scope key that can be revoked immediately. | Python, FastAPI, Streamlit, OIDC/PKCE, JWT, SCIM |
| [Secure RAG](https://github.com/DanMcB1/ai-secure-rag) | Document Q&A that only retrieves the files the signed-in person is allowed to see. | Python, Streamlit, TF-IDF (scikit-learn), access-control filter |
| [PII Unmasking Proxy](https://github.com/DanMcB1/ai-pii-unmasking-proxy) | Hides SSNs, card numbers, and other personal data from a model, then puts the originals back only for people who are allowed to see them. | Python, FastAPI, Streamlit, deterministic tokenization |
| [Approval Gate](https://github.com/DanMcB1/ai-approval-gate) | Pauses high-stakes AI actions until a person approves, and keeps that pause even if the process crashes. | Python, Temporal, Streamlit, mock Slack |

## Integration and infrastructure

| Project | What it does | Tech |
| --- | --- | --- |
| [Air-Gapped Deployer](https://github.com/DanMcB1/ai-airgapped-deployer) | One command installs a local AI stack on a sealed Kubernetes network and proves that calls out to the internet are blocked. | Helm, Kubernetes (kind), Terraform, NetworkPolicy, Streamlit |
| [Legacy Ingestor](https://github.com/DanMcB1/ai-legacy-ingestor) | Turns crooked scans, a mainframe file, a messy spreadsheet, and a memo into a searchable store, with a citation back to the source. | Python, Streamlit, Tesseract OCR, EBCDIC/COMP-3, TF-IDF, SQLite |
| [MCP-to-ERP Bridge](https://github.com/DanMcB1/ai-mcp-erp-bridge) | Translates clean AI tool calls (MCP) into the SOAP requests a legacy dealer system still speaks. A parts order still needs a human confirmation. | Python, FastAPI, Streamlit, MCP (JSON-RPC 2.0), SOAP 1.1 |
| [Local Triage Node](https://github.com/DanMcB1/ai-local-triage-node) | A small offline model screens incoming messages for personal data and routes them to the right desk, backed by checksums an F&I desk already trusts. | Python, Streamlit, Qwen2.5-1.5B Q4 GGUF (llama.cpp), regex + Luhn/ABA/VIN checks |

## Suggested pins

GitHub shows six pinned repositories on a profile. A balanced set — two from each group above — would be:

1. [ai-architecture-scoper](https://github.com/DanMcB1/ai-architecture-scoper) — the first customer conversation, turned into a plan
2. [ai-shadow-replay](https://github.com/DanMcB1/ai-shadow-replay) — prove the agent on past work before it goes live
3. [ai-sso-agent-broker](https://github.com/DanMcB1/ai-sso-agent-broker) — least-privilege keys for agents, not a shared login
4. [ai-approval-gate](https://github.com/DanMcB1/ai-approval-gate) — human sign-off that survives a crash
5. [ai-airgapped-deployer](https://github.com/DanMcB1/ai-airgapped-deployer) — install and prove an air-gapped stack
6. [ai-local-triage-node](https://github.com/DanMcB1/ai-local-triage-node) — a small local model, plus an honest scorecard
