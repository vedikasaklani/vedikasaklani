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

<table>
  <tr>
    <td valign="top" width="50%">
      <h3><a href="https://github.com/vedikasaklani/chatbot-and-mcp-agent-commerce">AI Commerce Agent: OAuth-Protected MCP + Razorpay</a></h3>
      <p><a href="https://drive.google.com/file/d/14w8QHVQa3Rht66EuI3LCjxFGqK71NW1n/view">Demo video</a></p>
      <p><code>FastAPI</code> <code>SQLAlchemy</code> <code>PostgreSQL</code> <code>Razorpay</code> <code>WorkOS OAuth</code> <code>MCP</code></p>
      <ul>
        <li>OAuth-protected MCP server (WorkOS bridge) lets external AI clients like Claude authenticate and place purchases through function calling.</li>
        <li>Multi-turn agent searches products, manages carts, and places orders with per-user memory, an audit log, and a decision record for each order.</li>
        <li>Razorpay checkout verifies webhook signatures and handles events idempotently. The server validates each payment instead of trusting model output.</li>
        <li>Deployed as three Render services, with Pytest coverage in GitHub Actions CI for webhook rejection, payment verification, and rollback cases.</li>
      </ul>
    </td>
    <td valign="top" width="50%">
      <h3><a href="https://github.com/vedikasaklani/mcp-server-exasol">MCP Server Trust Registry</a></h3>
      <p><a href="https://drive.google.com/file/d/1R9sLmjSL_2GYnYjBkptb0quM3jcn2iWk/view?usp=sharing">Demo video</a></p>
      <p><code>FastAPI</code> <code>PostgreSQL</code> <code>Exasol</code> <code>SQLAlchemy</code> <code>GitHub App Webhooks</code> <code>Alembic</code> <code>Docker</code></p>
      <ul>
        <li>Scans third-party MCP servers on every GitHub push with static rules and LLM behavioral analysis, then assigns a daily trust score.</li>
        <li>GitHub App webhook flow verifies signatures, clones private repositories with installation tokens, and runs a two-phase scan using Cisco <code>mcp-scanner</code>.</li>
        <li>Exasol SQL star schema receives best-effort PostgreSQL syncs, so analytics outages never fail a committed scan.</li>
      </ul>
    </td>
  </tr>
  <tr>
    <td valign="top" width="50%">
      <h3><a href="https://github.com/vedikasaklani/depSCAN">depSCAN</a></h3>
      <p><strong>Frontend Lead</strong></p>
      <p><code>React</code> <code>Recharts</code> <code>REST APIs</code></p>
      <ul>
        <li>Built the Project View with scan history, ecosystem filters, and NTIA compliance, plus a Vulnerability Dashboard with CVSS details, fix versions, dependency graph, and report export.</li>
        <li>Connected both views to live SBOM scan APIs and managed version control for a team of six.</li>
      </ul>
    </td>
    <td valign="top" width="50%">
      <h3><a href="https://github.com/vedikasaklani/tutorial-recommender">PDF-to-Video Learning Recommender</a></h3>
      <p><code>Python</code> <code>spaCy</code> <code>PyPDF</code> <code>Hugging Face API</code> <code>YouTube Data API</code></p>
      <ul>
        <li>NLP pipeline chunks PDFs with spaCy, ranks passages by embedding similarity, and asks an LLM to generate YouTube queries. Results are deduplicated and ranked.</li>
        <li>Chrome and Firefox extension recommends videos for the active PDF through a Flask REST API.</li>
      </ul>
    </td>
  </tr>
</table>
