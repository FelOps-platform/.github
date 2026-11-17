# FelOps

**FelOps** is a multi-tenant SaaS automation platform that lets teams interact with their business systems through natural language.

> **🚧 Project Status: Early Development**
> We have just kicked off development on FelOps. Most repositories in this organization are currently in their initial setup and scaffolding stages as we build out the core architecture.

---

### What is FelOps?

Instead of manually clicking through CRMs, ERPs, and email tools, users can simply ask an AI agent to get work done—for example:
> *"Create a new customer in Salesforce and send them a welcome email."*

FelOps interprets the request, checks the user's workspace permissions, plans the required steps, asks for human approval when needed, and executes the actions across connected integrations.

---

### Core Features

- **Multi-Tenant Workspaces & Granular RBAC:** Isolated workspaces with built-in roles (Owner, Admin, Member) and customizable permission bundles.
- **Knowledge-Driven AI Agents:** Train agents using website URLs, text snippets, and documents (PDF, DOCX, TXT) via RAG, guided by custom instructions and dynamic orchestration.
- **Integrations & MCP Actions:** Connect external platforms (CRM, ERP, Email) or custom APIs at the workspace level and expose authorized actions to agents via Model Context Protocol (MCP).
- **Human-in-the-Loop Controls:** Configure sensitive actions to require explicit human approval before execution, and allow team members to take over live agent conversations at any time.
- **Omnichannel Deployment:** Deploy agents via an embeddable website chat widget, a hosted chat page, WhatsApp, or custom frontends via API.
- **Mobile Companion & Localization:** Stay updated on urgent approvals and escalations on mobile, with full support for **English** and **Arabic**.

---

### How It Works

1. **Request:** A user sends a natural-language message through any connected channel.
2. **Context & Planning:** The agent retrieves relevant knowledge (RAG), checks conversation history, and selects authorized tools via MCP.
3. **Validation & Approval:** FelOps enforces workspace permissions and pauses for human approval if the action requires oversight.
4. **Execution:** The platform executes the task through the target integration and returns the result.
