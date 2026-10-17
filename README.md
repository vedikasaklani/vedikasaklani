<p align="center"><img src="assets/banner.svg" alt="Vedika Saklani, software engineer in the making"></p>

I build backend systems and full-stack features, from APIs and databases to CI and deployment.

BTech Computer Science (Cybersecurity) at **VIT**, Class of 2028 · CGPA **9.64**

[Email](mailto:ivedikasaklani@gmail.com) · [GitHub](https://github.com/vedikasaklani)

---

## About Me

I love falling into a rabbit hole and spending a whole week on one project. I like niche work and I like being a generalist. Anything that teaches me something new is fair game, which means I like a lot of things.

I'm looking to start contributing to open source soon. If you have a project and want a collaborator, [email me](mailto:ivedikasaklani@gmail.com) right now. No, actually, I'm interested, and I'll build. Bye!

---

## Skills

**Languages**

![Python](https://img.shields.io/badge/-Python-cfe8ff?style=for-the-badge)
![Java](https://img.shields.io/badge/-Java-ffd3e8?style=for-the-badge)
![JavaScript](https://img.shields.io/badge/-JavaScript-cfe8ff?style=for-the-badge)
![C](https://img.shields.io/badge/-C-ffd3e8?style=for-the-badge)
![C++](https://img.shields.io/badge/-C++-cfe8ff?style=for-the-badge)
![SQL](https://img.shields.io/badge/-SQL-ffd3e8?style=for-the-badge)

**Web and Backend**

![FastAPI](https://img.shields.io/badge/-FastAPI-cfe8ff?style=for-the-badge)
![Flask](https://img.shields.io/badge/-Flask-ffd3e8?style=for-the-badge)
![Django](https://img.shields.io/badge/-Django-cfe8ff?style=for-the-badge)
![React](https://img.shields.io/badge/-React-ffd3e8?style=for-the-badge)
![SQLAlchemy](https://img.shields.io/badge/-SQLAlchemy-cfe8ff?style=for-the-badge)
![OAuth](https://img.shields.io/badge/-OAuth-ffd3e8?style=for-the-badge)
![REST_APIs](https://img.shields.io/badge/-REST_APIs-cfe8ff?style=for-the-badge)

**AI and LLM**

![MCP](https://img.shields.io/badge/-MCP-ffd3e8?style=for-the-badge)
![LLM_Tool_Calling](https://img.shields.io/badge/-LLM_Tool_Calling-cfe8ff?style=for-the-badge)
![Prompt_Engineering](https://img.shields.io/badge/-Prompt_Engineering-ffd3e8?style=for-the-badge)
![Hugging_Face_API](https://img.shields.io/badge/-Hugging_Face_API-cfe8ff?style=for-the-badge)
![spaCy](https://img.shields.io/badge/-spaCy-ffd3e8?style=for-the-badge)

**Data and Tools**

![PostgreSQL](https://img.shields.io/badge/-PostgreSQL-cfe8ff?style=for-the-badge)
![Docker](https://img.shields.io/badge/-Docker-ffd3e8?style=for-the-badge)
![AWS](https://img.shields.io/badge/-AWS-cfe8ff?style=for-the-badge)
![GitHub_Actions](https://img.shields.io/badge/-GitHub_Actions-ffd3e8?style=for-the-badge)
![Git](https://img.shields.io/badge/-Git-cfe8ff?style=for-the-badge)
![Claude_Code](https://img.shields.io/badge/-Claude_Code-ffd3e8?style=for-the-badge)

---

## Projects

### [AI Commerce Agent: OAuth-Protected MCP + Razorpay](https://github.com/vedikasaklani/chatbot-and-mcp-agent-commerce)
[Demo video](https://drive.google.com/file/d/14w8QHVQa3Rht66EuI3LCjxFGqK71NW1n/view)

`FastAPI` `SQLAlchemy` `PostgreSQL` `Razorpay` `WorkOS OAuth` `MCP`

- OAuth-protected MCP server (WorkOS bridge) that lets external AI clients like Claude authenticate and place purchases via function calling.
- Multi-turn agent that searches products, manages the cart and places orders, with per-user memory, a full audit log and a decision record per order.
- Razorpay checkout with webhook signature verification and idempotent event handling. The server validates every payment itself rather than trusting model output.
- Deployed as three Render services, with a Pytest suite in GitHub Actions CI (webhook rejection, payment verification, rollback on provider failure or order-cap breach).

### [MCP Server Trust Registry](https://github.com/vedikasaklani/mcp-server-exasol)
[Demo video](https://drive.google.com/file/d/1R9sLmjSL_2GYnYjBkptb0quM3jcn2iWk/view?usp=sharing)

`FastAPI` `PostgreSQL` `Exasol` `SQLAlchemy` `GitHub App Webhooks` `Alembic` `Docker`

- Registry that scans third-party MCP servers on every GitHub push (static rules + LLM behavioral analysis) and assigns a daily trust score.
- GitHub App webhook flow (signature verification, private-repo cloning via installation tokens) and a two-phase scan pipeline integrating the Cisco `mcp-scanner`.
- SQL star schema in an Exasol warehouse, fed by a best-effort PostgreSQL to Exasol sync so an analytics outage never fails a committed scan.

### [depSCAN](https://github.com/vedikasaklani/depSCAN)
Frontend Lead

`React` `Recharts` `REST APIs`

- Built the Project View (scan history, ecosystem filtering, NTIA compliance overview) and the Vulnerability Dashboard (CVE table with CVSS, affected packages, fix versions, dependency graph, report export).
- Wired both views to live SBOM-scan APIs and managed version control for a team of 6.

### [PDF-to-Video Learning Recommender](https://github.com/vedikasaklani/tutorial-recommender)

`Python` `spaCy` `PyPDF` `Hugging Face API` `YouTube Data API`

- NLP pipeline: chunks PDFs with spaCy, ranks chunks by embedding similarity, and prompts an LLM to generate YouTube queries. Results are deduplicated and ranked.
- Chrome/Firefox extension that recommends videos for the active tab's PDF via a Flask REST API.
