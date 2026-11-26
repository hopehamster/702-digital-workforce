# Blueprint Summary — 702 AI Services Digital Workforce Architecture

*This is a summary of a Deep Research report ("702 AI Services Digital Workforce Architecture Blueprint") produced in Michael's ChatGPT in November 2025. The full report lives in that ChatGPT conversation; only its summary was shared, and this document records the summary faithfully — findings, recommendations, and estimates are the report's, presented as planning material, not measured production results.*

## The headline discovery

> A digital employee doesn't need a continuously running computer. It needs a persistent identity with access to computing resources on demand.

The employee retains its professional skills, memory, personality, documents, permissions, and assignments, while computing resources are provisioned only when the employee has work to do. Thousands of digital employees could therefore be maintained without maintaining thousands of computers — **a factory that manufactures digital employees, not individually creating them one by one.**

## Recommended stack

| Layer | Recommendation | Role |
|---|---|---|
| Orchestration | **LangGraph** | Primary orchestration framework |
| Complex assignments | **Deep Agents** | Complex professional work |
| Hosted Linux | **Cloudflare Sandbox** | Primary hosted Linux environment |
| Employee office | **Cloudflare Computer** | Adopt stable components selectively — persistent workspace (memory, files, skills, documents) |
| Local compute | **Unkernel** | Optional local computing on customer hardware |
| Browser work | **Cloudflare Browser Run** | Primary browser automation — access to authorized web applications where no API exists |
| Identity & data | **Supabase / PostgreSQL** | Employee identity, memory, and customer data |
| Integrations | **Nango** | Business application integrations and credentials |
| Reliability | **Temporal** | Advanced workflow reliability as the business grows |
| Evaluation | **Langfuse** | Employee performance evaluation and monitoring |
| Billing | **Stripe** | Workforce subscriptions and usage billing |

The research validates the overall vision but changes the priority of two technologies: Unkernel moves from central to *optional local computing*, and Cloudflare Sandbox becomes the *primary hosted Linux environment*. The existing LangGraph + Deep Agents layer is retained as the intelligence and orchestration layer.

## How the pieces combine

- **Unkernel** gives a digital employee a *local computer* — customer-powered Linux on the customer's own workstation, with the privacy benefit that customer data stays local.
- **Cloudflare Computer** gives the employee a *persistent, professional office* — a workspace that exists independently of any execution environment, so an employee can start a task in a lightweight shell, escalate to a full Linux container, and resume the same files later. Stable components (persistent filesystem, Code Mode execution, agent tools, Git integration, skill bundling, observability) are the foundation; the full Linux container backend, lightweight shell backend, and integrated browser are documented as experimental and treated as future upgrades. Documented workspace storage is approximately 10 GB, and credentials/long-lived secrets should not be stored in the workspace.
- **Professional skill packages** are mounted into the workspace as bundled skills and templates: professional skills (correspondence, scheduling, reporting), company policies, customer-specific operating procedures, application access (email, calendar, documents, CRM), assignments, memory, and audit logs. A master professional configuration is maintained centrally while each leased employee keeps an isolated, customer-specific workspace — making mass deployment practical.
- **Synchronization and execution coordination** between the local (Unkernel) and office (Cloudflare) environments still needs to be built; it is an explicit work item, not a solved problem.

## Estimated operating costs

Estimated *direct monthly technology cost per active employee* (research-based planning estimates, not measured production costs; excludes support, onboarding, sales, and other costs):

| Worker type | Est. cost / month |
|---|---|
| Light routine worker | $4–$8 |
| Standard office worker | $7–$15 |
| Browser-intensive worker | $12–$30 |
| Software engineer | $20–$60 |
| Premium intelligence worker | $30–$100+ |

Set against catalogue pricing of $599–$10,000 per employee per month, the direct-cost margin is wide; the real costs to manage are supervision, quality, and customer success.

## What else the report covers

Detailed comparisons of competing agent frameworks; employee memory and persistent-identity architecture; database schemas and repository structure; professional skill packages and certification systems; progressive employee autonomy and promotions; customer onboarding and offboarding; security, credential management, and access permissions; local/cloud computer synchronization; cost projections for 10, 100, and 1,000 customers; an implementation roadmap and technical acceptance tests; and complete workflows for administrative, financial, engineering, and project-management employees.

## The four foundational documents

The research recommends turning the blueprint into four engineering documents, which form Phase 0 of the program:

1. **Master Architecture Specification** — the definitive technology stack.
2. **Digital Employee Standard** — what every digital employee must possess.
3. **Digital Workforce Factory Specification** — how we manufacture, configure, certify, and deploy employees.
4. **Engineering Implementation Plan** — a precise, phased construction plan with acceptance tests.

The research is complete, but the proposed integrations have **not yet been benchmarked or tested** — proving them is the work the program plan sequences.
