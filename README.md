<p align="center"><img src="assets/banner.png" alt="Vedika Saklani, software engineer in the making"></p>

## About me

I build backend systems and full-stack features, from APIs and databases to CI and deployment. 

BTech Computer Science (Cybersecurity) at **VIT**, Class of 2028 

[Email](mailto:ivedikasaklani@gmail.com) · [GitHub](https://github.com/vedikasaklani) · [LinkedIn](https://www.linkedin.com/in/vedika-saklani-2a1598375)

---

## What I'm Working On

- **AI engineering:** learning how to build production-ready AI systems
- **[Folio](https://github.com/vedikasaklani/folio):** a drawing and editing app with real-time sharing, which I'm building and learning from
- Finding my first open source project to contribute to

---

## Skills

**Languages**

![Python](assets/skills/python.svg?v=8) ![Java](assets/skills/java.svg?v=8) ![JavaScript](assets/skills/javascript.svg?v=8) ![C](assets/skills/c.svg?v=8) ![C++](assets/skills/cpp.svg?v=8) ![SQL](assets/skills/sql.svg?v=8)


**Web and Backend**

![FastAPI](assets/skills/fastapi.svg?v=8) ![Flask](assets/skills/flask.svg?v=8) ![Django](assets/skills/django.svg?v=8) ![React](assets/skills/react.svg?v=8) ![SQLAlchemy](assets/skills/sqlalchemy.svg?v=8) ![OAuth](assets/skills/oauth.svg?v=8) ![REST_APIs](assets/skills/rest-apis.svg?v=8)

**AI and LLM**

![MCP](assets/skills/mcp.svg?v=8) ![LLM_Tool_Calling](assets/skills/llm-tool-calling.svg?v=8) ![Prompt_Engineering](assets/skills/prompt-engineering.svg?v=8) ![Hugging_Face_API](assets/skills/hugging-face-api.svg?v=8) ![spaCy](assets/skills/spacy.svg?v=8)

**Data and Tools**

![PostgreSQL](assets/skills/postgresql.svg?v=8) ![Docker](assets/skills/docker.svg?v=8) ![AWS](assets/skills/aws.svg?v=8) ![GitHub_Actions](assets/skills/github-actions.svg?v=8) ![Git](assets/skills/git.svg?v=8) ![Claude_Code](assets/skills/claude-code.svg?v=8)

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
