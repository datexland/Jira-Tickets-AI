# Jira Ticket Creator — AI Agent Skill

> Stop writing incomplete tickets. Let your AI agent interview you like a Senior Product Owner and generate production-ready Jira stories in seconds.

---

## Why This Exists

How many times has your team shipped a ticket with no business value, missing dependencies, or zero Definition of Done?

This skill plugs directly into your AI coding agent and transforms it into an assertive **Technical Product Owner** — one that pushes back on vague requirements, tracks upstream blockers, and enforces your team's standards on every single ticket.

**No more back-and-forth. No more half-baked stories. Just ship.**

---

## What You Get

| Feature | Description |
|---|---|
| **Guided Interview** | The agent asks the right questions so you never miss critical context |
| **Strict Template Enforcement** | Every ticket includes User Story, DoR, and DoD — no exceptions |
| **Blocker Detection** | Automatically flags tickets as BLOCKED when upstream dependencies are incomplete |
| **Instant Markdown Output** | Copy-paste ready for Jira or saved directly as a `.md` file |
| **Works with Any LLM** | Cursor, Antigravity, Claude Code — your team's choice |

---

## Get Started in 2 Minutes

**1. Clone the repo**
```bash
git clone https://github.com/datexland/Jira-Tickets-AI.git
cd Jira-Tickets-AI
```

**2. Open your IDE**

Launch **Cursor**, **Antigravity**, or **Claude Code** — whichever your team uses.

**3. Choose your LLM**

We recommend **Gemini Flash** for fast, intelligent drafting during demos and daily use.

**4. Open the Agent tab and type:**

```
Hey man, could you help me to create a Jira ticket?
```

That's it. The agent takes over from here.

**5. Follow the interview**

The agent will guide you through:
- **Title & Persona** — Who is this for and what are they doing?
- **Business Value** — Why does this matter to the business?
- **Background & Dependencies** — What are the upstream blockers? Any Confluence links?
- **Technical Blueprint** — Logic, naming conventions, security & access requirements.
- **DoR & DoD Validation** — Is this ticket actually ready to be worked on?

---

## Demo

Watch the full workflow in action — from a single prompt to a complete, production-ready Jira ticket:

![Jira Ticket Creator Demo](demo_video/jira_demo.gif)

---

## Example Output

```markdown
#### Title: Installing Python Dependencies via plugins.zip

#### Description
As a Data Engineer, I want to install the `apache-airflow-providers-dbt-cloud==4.4.2`
dependency via a `plugins.zip` file, So that we can run dbt jobs from our MWAA
Airflow environment which is currently restricted within a private network.

#### Background
The MWAA environment is hosted within a private network without public internet
access, preventing the automatic download of Python packages during environment
startup. This task involves creating and configuring the `plugins.zip` package
to include the necessary dbt-cloud provider.

#### Definition of Ready (DoR)
- [x] Access to required systems/sources (S3/MWAA) is granted
- [x] Documentation or designs are available and linked in Background
- [x] Upstream dependencies are identified and complete

#### Definition of Done (DoD)
- [ ] Code follows naming conventions (e.g., `plugins.zip`)
- [ ] Unit tests passed (verified by successful DAG import in MWAA)
- [ ] Deployment completed and observability verified in MWAA logs
```

---

## Who Should Use This

- **Data Engineers** building dbt models, pipelines, and integrations
- **Platform Engineers** managing infrastructure and access changes
- **Tech Leads** who are tired of refining vague tickets before sprint planning
- **Any team** that values consistency, clarity, and speed

---

> Built for Data & Platform Engineering teams who take their craft seriously.
