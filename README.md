# IS373 Individual Record: Alex Wiemer

**Course:** IS373 Content Management Systems, NJIT, Fall 2026 · **GitHub:** [ACW900](https://github.com/ACW900)

This record holds my two individual deliverables. My group work (Deliverable 3) is in my team's shared record.

| Section | Contents |
|---|---|
| [1. Individual portfolio + career research](#1-individual-portfolio--career-research) | Employer postings, two directions compared, target reader, evidence map, outline, layouts |
| [2. Individual RAG app + technical research](#2-individual-rag-app--technical-research) | Reader/question, sources, vector/graph/keyword comparison, architecture, evaluation questions, checks, hosting |

**Status labels:** `planned` · `observed locally` · `observed in CI` · `observed hosted`. A plan, sketch or expected answer is not an executed test.

**Stage:** Review 1 (Plan), due Nov 17, 2026. No hosted app is required yet; planned URLs are labeled.

---
## 1. Individual portfolio + career research

### Index

| Item | Where | Status |
|---|---|---|
| 4 employer posting records | [A](#a-employer-posting-records) | checked Nov 16, 2026 |
| Comparison of 2 directions | [B](#b-comparing-two-directions) | written |
| Target reader + direction | [C](#c-target-reader-and-direction) | chosen (provisional) |
| Private reflection | [D](#d-private-reflection-not-public) | private |
| Responsibility → evidence map | [E](#e-responsibility-to-evidence-map) | written (each row labeled observed / planned) |
| Portfolio outline | [F](#f-portfolio-outline) | written; site planned for Build |
| Two layout options + choice | [G](#g-two-lightweight-layouts) | wireframed; Layout A chosen |
| Peer check + changed/checked/next | [H](#h-peer-check-and-changed--checked--next) | peer check pending |

---

### A. Employer posting records

*All three were opened on the employer's own site on **Nov 16, 2026**. Responsibilities are paraphrased. Re-open each one and add the date **you** checked it.*

#### P1: Forward Deployed Engineer (FDE), OpenAI *(required FDE reference)*

| Field | Notes |
|---|---|
| Role family | **Forward deployed engineering** |
| Employer / industry | OpenAI · AI research and deployment |
| URL | https://openai.com/careers/forward-deployed-engineer-(fde)-sf-san-francisco/ |
| Date checked | Nov 16, 2026 |
| Posted / deadline / status | Not stated on the page · open when checked |
| Location / arrangement | San Francisco · hybrid, 3 days/week in office · **up to 50% travel** · relocation offered |
| Level / eligibility | **Senior: 5+ years** engineering or deployment experience with customer-facing work. **Longer-term reference, not something I qualify for now.** |
| 3 responsibilities (my words) | 1. Take customer AI deployments from first prototype to stable production. 2. Work inside customer teams to understand their needs and help them adopt what's built. 3. Turn repeated solutions into reusable tools/playbooks and send field feedback to product and research. |
| Required | 5+ yrs incl. customer-facing work; production frontend + backend code (Python/JS); has built or deployed LLM-powered systems |
| Preferred | Delivering complex systems in ambiguous settings; clear communication with engineers and customers |
| Short excerpt | "Own technical delivery across multiple deployments from first prototype to stable production" *(In this role you will)* |
| Something I've actually done | Took Save Point from spec to merged, tested features through issues/PRs with CI (App Studio APP-001–003) |
| Gap | No customer-facing delivery; no LLM-powered system yet |
| My impression *(my assumption about fit, not a posting fact)* | From reading the role description, this job seems very based around results and not very structured or boxy. |
| Next action (dated) | Build the RAG app's first real source → answer path by **Nov 24** (Review 2) |

#### P2: AI Engineer (MLOps) Intern, New York Life *(junior / internship)*

| Field | Notes |
|---|---|
| Role family | **Platform / MLOps** (with AI engineering) |
| Employer / industry | New York Life Insurance Company · financial services / insurance |
| URL | https://careers.newyorklife.com/careers/job/43624352-2027-technology-data-ai-ventures-summer-internship-program-ai-engineer-mlops-intern-new-york-new-york-united-states |
| Date checked | Nov 16, 2026 |
| Posted / deadline / status | Requisition 94548 · deadline not stated on the employer page · **Likely closed:** the direct page still loaded Nov 16, but the TDAV internships no longer appear in New York Life's job search, and one third-party listing said it expired Nov 15. It still works as research evidence; just don't count on applying. |
| Location / arrangement | New York, NY · hybrid, 3 days/week on-site · 11 weeks, May 25 – Aug 6, 2027 · $30–35/hr + $3,000 bonus |
| Level / eligibility | **Internship.** Bachelor's/master's student graduating **Dec 2027 or May 2028**; must be authorized to work in the U.S. (no sponsorship, no OPT/CPT). **My expected graduation: Fall 2027 / Spring 2028, which matches. Confirm the exact term and my work authorization when applying.** |
| 3 responsibilities (my words) | 1. Help deploy ML and generative AI models into production with Python APIs. 2. Improve MLOps/DevOps platforms with dashboards and monitoring (e.g. New Relic). 3. Contribute to automation that keeps models reliable at scale. |
| Required | CS/data/AI-related degree in progress; Python; APIs; automated testing; DevOps tools (examples given: EKS, CI/CD, New Relic) |
| Preferred | Not separately listed |
| Short excerpt | "designing and testing new patterns for model deployment using Python APIs" *(What You'll Do, example projects)* |
| Something I've actually done | Built a QA → production **CI/CD pipeline** (Docker image → GHCR → SSH deploy, health check, rollback) for acw33firstliveproj.online; automated tests + CI in Save Point |
| Gap | No ML/LLM model in production; no monitoring/observability tool; no Kubernetes/EKS |
| My impression *(my assumption about fit, not a posting fact)* | I like the "What You'll Do" section because it gives actual tasks for what you're supposed to be doing. I think this is something the OpenAI posting is missing. |
| Next action (dated) | Deploy the RAG app through my existing pipeline with a health check and basic logging by **Dec 3** (Review 3) |

#### P3: Product Engineer, Computer Use, Anthropic *(alternative direction)*

| Field | Notes |
|---|---|
| Role family | **AI product engineering** |
| Employer / industry | Anthropic · AI research and products |
| URL | https://job-boards.greenhouse.io/anthropic/jobs/5238637008 |
| Date checked | Nov 16, 2026 |
| Posted / deadline / status | Not stated · open when checked |
| Location / arrangement | San Francisco, **New York City**, or Seattle · in office at least 25% of the time |
| Level / eligibility | **Experienced:** asks for zero-to-one product ownership and shipping to external users. **Longer-term reference.** Visa sponsorship possible. |
| 3 responsibilities (my words) | 1. Own computer-use/browser-control product features end to end: scope, build, ship, measure, iterate. 2. Find and fix reliability problems in the agent system that block real use. 3. Turn vague user pain points into concrete features, using usage data to prioritize. |
| Required | Shipped a product 0→1 with end-to-end ownership; strong full-stack web skills; hands-on with LLM APIs/prompting/agents; iterating on external user feedback |
| Preferred | Product design instincts; browser/desktop automation; building evals; light data analysis (SQL); agent loops/guardrails |
| Short excerpt | "Translate fuzzy user pain points into concrete, shippable features for knowledge workers" *(Key responsibilities)* |
| Something I've actually done | Designed Save Point around a specific user ("a gamer looking for news about his favorite games") and made product decisions in its SPEC; full-stack FastAPI + templates + SQLite |
| Gap | No LLM API work yet; no real external users or usage data; no evals yet |
| My impression *(my assumption about fit, not a posting fact)* | I feel this is the job I align with most. It describes things I've been doing for years now, and the information is very cleanly laid out. *(Name which things specifically, e.g. troubleshooting, building full-stack apps, designing for a user.)* |
| Next action (dated) | Write and run the RAG app's 5 evaluation questions and record actual results by **Dec 3** |

#### P4 (extra, open now): AI/Automation Development Intern – Assessment & Authorization, Leidos *(AI automation)*

*An extra posting beyond the required three. It matches my AI automation goal and was **open with applications accepted** when checked.*

| Field | Notes |
|---|---|
| Role family | **AI automation** (close to data/evaluation and security in the handout's families) |
| Employer / industry | Leidos · defense / government IT contractor (SMIT contract) |
| URL | https://leidos.wd5.myworkdayjobs.com/External/job/6314-RemoteTeleworker-US/AI-Automation-Development-Intern---Assessment---Authorization_R-00195319 |
| Date checked | Nov 16, 2026 |
| Posted / deadline / status | Originally posted Nov 6, 2026 · req R-00195319 · **accepting applications** when checked · no close date stated (Leidos only promises at least 3 days open, so apply soon) |
| Location / arrangement | **Remote (US)** · full time · internship dates **not stated**, so confirm it's summer 2027 |
| Level / eligibility | **Internship**: degree in CS/IT/cybersecurity/related (junior or senior standing preferred). **Must be a U.S. citizen (I am ✅) and able to get a Secret clearance** (involves a background check). Listed range $48,100–$86,950 (annualized). |
| 3 responsibilities (my words) | 1. Write automation scripts (Python, PowerShell, JS or Bash) that speed up security-authorization (RMF) paperwork and workflows. 2. Help build and test AI-enabled tools that analyze security controls and authorization packages. 3. Document what's built, join code reviews, and test/QA the automation. |
| Required | Scripting in Python, PowerShell, JavaScript or Bash; clean documented code; basic automation concepts; communication; **U.S. citizen + Secret clearance eligibility** |
| Preferred | AI/ML libraries or OpenAI API; AI coding assistants; RPA tools; LLMs for documents; Git/GitHub; REST APIs; cloud; **DevOps and CI/CD**; SQL/NoSQL; Agile |
| Short excerpt | "Develop and maintain automation scripts to streamline RMF processes and A&A workflows" *(Primary Responsibilities)* |
| Something I've actually done | IT340 Bash scripts (cron logging of uptime/memory/disk; interactive timesheet); GitHub Actions CI/CD pipeline; Git/GitHub with issues and PRs; JavaScript (Node/Express) |
| Gap | No AI/LLM tooling built yet; no PowerShell; no cybersecurity compliance (NIST RMF) background |
| My impression *(my assumption about fit, not a posting fact)* | This one interests me because it mentions testing in a workplace setting, and I'm not sure what that would involve. I have experience troubleshooting and finding bugs, but I don't know if that's what's required. |
| Next action (dated) | Citizenship confirmed. Confirm the summer 2027 dates, then apply **this week (by Nov 20)**. Mention the IS373 RAG app only once it's actually built. |

**Note on these sources:** P1 and P3 came from the instructor's career handout source leads (checked there Nov 3). P2 came from a web search and was confirmed on New York Life's own careers site. P4 came from a public internship tracker (github.com/zshah101/Automated-List-Of-Summer-2027-and-Fall-2026-Tech-Internships) and was confirmed on Leidos's own Workday page. Four postings are a small sample, not proof of what the whole job market wants.

---

### B. Comparing two directions

| Question | **Direction 1: Platform / MLOps** (P2) | **Direction 2: AI product engineering** (P3) |
|---|---|---|
| What would I do regularly? | Deploy models/services, automate pipelines, monitor reliability | Build user-facing AI features end to end, fix reliability issues, iterate from usage |
| What attracts me / what doesn't? | I feel like this is something I could go into with more confidence. I have full-stack experience and could be on the ground floor of AI integration in web development. The New York Life posting also lists actual tasks ("What You'll Do"), so I can picture the work. | This is the posting I align with most; it describes work I already do, and it's clearly laid out. But I feel like I don't know much about real AI skills yet; the only things I know are how to prompt and the basics of how LLMs work. It's also a senior role, not an entry point yet. |
| What can I show today? | CI/CD pipeline with QA/prod + rollback; Docker; HTTPS with Caddy; calculator deploy; IS373 practical test on secure deployment | Save Point: user-focused design, auth, roles, tests, CI |
| Biggest gap | ML/LLM in production; monitoring; Kubernetes | LLM APIs; real users; evals |
| Can IS373 help? | Yes: hosting the RAG app with persistence, health checks, secrets | Yes: the RAG app's user question → answer + evaluation |
| Junior entry point found? | **Yes**: P2 internship | Not yet: P3 is senior |

**FDE (P1)** combines both: building and deploying for a customer. It's a useful long-term reference, but it needs years of experience and heavy travel.

---

### C. Target reader and direction

**Provisional direction: a product-minded engineer who can also ship it.**
- **Where I lean:** AI product engineering (P3). It's the posting I align with most: understanding a user's problem, building the feature front to back, and improving it.
- **Where I'll start:** DevOps / AI automation internships (P2, P4). They have real entry points for summer 2027, and they match my strongest evidence (my CI/CD pipeline, Bash automation, troubleshooting).
- **Why both:** many people enter through infrastructure and automation and move toward product work. Knowing how to deploy and run what I build also makes me a stronger product engineer.
- **Longer term:** AI automation / AgentOps and AI infrastructure; FDE (P1) is a possible later path, since it combines building for users with deploying.

**Near-term target:** summer 2027 internships in AI automation, AI engineering, DevOps or cloud.

**Primary reader:** an **internship reviewer hiring for AI automation, AI engineering or DevOps intern roles** (like P4 and P2).

**What they should understand after one visit:**
> "This student builds useful apps for real users, and can take them from code to a tested, live deployment, with the evidence to show it."

**What I should *not* claim:** professional production experience, finished features that aren't built, or skills I haven't shown (Kubernetes, ML training).

---

### D. Private reflection (not public)

*My private reflection (two directions, my leaning, evidence, gap, dated action, and what the research changed) is submitted in the Canvas text box, not published here.*

---

### E. Responsibility to evidence map

| Employer responsibility (source) | Evidence I'll feature | Status |
|---|---|---|
| Deploy AI/ML systems to production with Python APIs (**P2**) | RAG app (FastAPI) deployed through my CI/CD pipeline to a live HTTPS URL | planned (Build, Nov 24) |
| Improve reliability with monitoring and automation (**P2**) | Existing pipeline: automated tests, image smoke test, health check, automatic rollback. Debugged a Caddy 502 by reading the logs and fixing a container missing from the Docker network. IT340 cron scripts logging uptime/memory/disk. Add basic logging/health page for the RAG app. | pipeline + 502 fix **observed hosted**; RAG monitoring planned |
| Take a deployment from prototype to stable production (**P1**) | Save Point: issue → branch → PR → CI for each feature; RAG app going Plan → Build → Checked Release | App Studio **observed in CI**; RAG planned |
| Turn user pain points into features (**P3**) | Save Point's user, promise, and design decisions in its SPEC; RAG reader/question (patch notes) | SPEC done; RAG planned |
| Build evals / measure quality (**P3** preferred) | RAG evaluation: 5 questions with expected sources, actual results, missing-evidence case | planned (Dec 3) |
| Work with a team (**P1**) | Group project case study naming my contribution | planned |
| Understand users and build full stack (**P3**) | GameAtlas: frontend → Express API → MongoDB across separate VMs | **observed** (Spring 2026, IT 340) |

**Evidence links:**
- CI/CD pipeline: https://github.com/ACW900/IS-373-TEST-CICD · live: https://acw33firstliveproj.online (QA: https://qa.acw33firstliveproj.online)
- Save Point (App Studio): https://github.com/ACW900/IS373_APPSTUDIO *(local app; not hosted yet)*
- GameAtlas: https://github.com/ACW900/IT340-Group-Project-
- Planned portfolio URL: https://acw33firstliveproj.online *(planned; not built yet)*

---

### F. Portfolio outline

| Page / section | What goes there |
|---|---|
| **Home / intro** | Name, one-line direction ("I build apps people use, and ship them with automated pipelines"), 3–4 featured projects, links to GitHub/LinkedIn/resume |
| **Full-stack app case study** | GameAtlas (frontend → Express API → MongoDB across VMs) and/or Save Point: who it's for, what I built, what I'd fix next |
| **RAG app case study** | Problem (returning players + patch notes), architecture, source → answer trace, evaluation results, limits, **link to the live chat** |
| **Deployment / platform case study** | My CI/CD pipeline: QA → production, rollback, health checks, what broke and how I fixed it |
| **Group project case study** | The shared system and **my named contribution** (with PR/issue links) |
| **About + contact** | Short background, what I'm learning next, professional contact route |

**Rules for the site:** no account needed to view it; mobile-friendly; keyboard-navigable; working links; anything unfinished labeled honestly.

**Where it will live (planned):** `https://acw33firstliveproj.online` (replacing the current placeholder page), deployed through my existing `qa` → `main` pipeline. *Confirm this is what you want.*

---

### G. Two lightweight layouts

*Same content, two arrangements.*

**Layout A: Evidence-first**

![Layout A: evidence-first wireframe with a short intro and three project cards](images/layout-a-evidence-first.svg)

**Layout B: Story-first**

![Layout B: story-first wireframe with a photo, long intro, journey timeline, and projects lower down](images/layout-b-story-first.svg)

*Wireframes made with Claude from my layout descriptions; I chose the content and the comparison.*

| | **Layout A: Evidence-first** | **Layout B: Story-first** |
|---|---|---|
| Home page | Short intro line → **grid of project cards** (each: one sentence, a "live demo" link, a "how it works" link) | Longer intro about my path → projects appear further down as a narrative |
| Case studies | Separate page per project, with the same headings each time (Problem · Approach · Evidence · Limits) | One long scrolling page telling the story in order |
| Good for | A reviewer skimming 30 seconds for proof | A reader who wants to understand me as a person |
| Risk | Can feel impersonal | Evidence is buried; reviewers may leave before finding it |

**How the postings drove these design decisions:**

| Employer evidence | Portfolio decision |
|---|---|
| P3: turn user pain points into shippable features | Every project card starts with **"For: …"** (who it's for) |
| P2 / P4: deploy, automate and test reliably | Every project card shows **"Ships via: …"**, with a deployment case study |
| P1: prototype → stable production | The RAG case study shows Plan → Build → Checked Release, with evidence at each stage |
| P2 / P4 are internships with reviewers who skim | Evidence-first layout: live demos and code one click from the homepage |

**Provisional choice: Layout A (evidence-first).** My reader is an internship reviewer checking for proof that I can build *and* ship, so the live demos and evidence need to be one click away. Each project card can show both sides: "who it's for" and "how it's deployed." *This is a design hypothesis; the peer check at Improve will test it.*

---

### H. Peer check and changed / checked / next

**Peer check:** a real classmate reviewed my postings, target reader (C) and layouts (G): *"Looking at these postings, does my target reader and featured evidence make sense?"*
- Peer: [name] · Date: [ ]
- What they said: [ ]
- My decision / what I changed: [ ]

**Changed:** researched 4 employer postings across 4 role families (FDE, platform/MLOps, AI product engineering, AI automation); compared two directions; chose a provisional direction (lean toward AI product engineering, enter through DevOps / AI automation internships) and reader (AI automation / AI engineering / DevOps internship reviewer); mapped responsibilities to evidence; outlined the site; wireframed two layouts and chose evidence-first.
**Checked (actually done):** opened all 4 postings on the employers' own sites on Nov 16, 2026 and confirmed my notes and excerpts match. Peer check: see above.
**Next:** build the portfolio foundation (intro, navigation, labeled project placeholders) on acw33firstliveproj.online for **Build, Nov 24**; apply to the Leidos internship (P4) by Nov 19.

**AI help:** Claude (an AI assistant) found and summarized the job postings, drafted this section's structure, and made the two layout wireframes from my descriptions. I opened and checked every posting myself, wrote my impressions of each, chose the direction (from options Claude explained), and chose the layout.

---

## 2. Individual RAG app + technical research

### Index

| Item | Where | Status |
|---|---|---|
| Research question + reader | [A](#a-reader-and-question) | planned |
| Technical sources + dates checked | [B](#b-technical-sources) | planned |
| Vector / graph / keyword comparison | [C](#c-comparing-approaches) | planned |
| Architecture choice | [D](#d-chosen-architecture) | planned |
| Source manifest | [E](#e-source-manifest) | planned |
| Sample representation (source → chunk → answer trace) | [F](#f-one-source-traced-through-the-system) | planned (illustrative, not executed) |
| Evaluation questions | [G](#g-evaluation-questions) | planned |
| Stories / checks | [H](#h-observable-stories-and-checks) | planned |
| Hosting, cost and limits | [I](#i-hosting-cost-and-limits) | planned |
| Changed / checked / next | [J](#j-changed--checked--next) | — |

**Status labels I'll use:** `planned` · `observed locally` · `observed in CI` · `observed hosted`. A sketch or expected answer is **not** an executed result.

---

### A. Reader and question

**Product:** a RAG feature added to **Save Point**, my existing FastAPI app (App Studio repo: https://github.com/ACW900/IS373_APPSTUDIO).

**Why this fits:** Save Point's promise is *"New patch? Get caught up from the last time you played."* My App Studio SPEC records that the app has no real news source yet. RAG over official patch notes fills that gap.

**One-sentence goal:**
> Save Point helps **a returning player of [GAME]** answer **"what changed since I last played?"** questions using **[about 5] official [GAME] patch notes**.

**Reader:** a player who stopped for a few weeks or months and wants to know what changed for the characters, weapons, items or modes they care about, without reading every patch note.

**Research question:** For short, versioned patch notes, does vector retrieval find the right changes for plain-language questions better than a keyword baseline? What would a graph (patch → changed thing → type of change) add for relationship questions?

---

### B. Technical sources

*Read each one yourself and fill in the date. Only write down claims you actually saw in the source.*

| # | Source | What I'm using it for | Date checked | What I learned (my words) |
|---|---|---|---|---|
| T1 | Course research handout: https://github.com/kaw393939/is373-studio/blob/main/docs/handouts/database-rag-research.md | Required concepts, comparison table | [date] | [ ] |
| T2 | Lewis et al. (2020), *Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks*: https://arxiv.org/abs/2005.11401 | Where the term "RAG" comes from | [date] | [ ] |
| T3 | SQLite FTS5 (full-text search): https://www.sqlite.org/fts5.html | Keyword baseline in the database I already use | [date] | [ ] |
| T4 | sqlite-vec: https://github.com/asg017/sqlite-vec | Vector search inside SQLite, so no new database server | [date] | [ ] |
| T5 | Qdrant documentation: https://qdrant.tech/documentation/ | Alternative: dedicated vector database + metadata filtering | [date] | [ ] |
| T6 | Neo4j documentation: https://neo4j.com/docs/ | Graph database alternative (also supports vector indexes) | [date] | [ ] |
| T7 | Course chunking handout: https://github.com/kaw393939/is373-rag/blob/main/docs/students/chunking.md | Chunking experiment design | [date] | [ ] |
| T8 | Course embeddings handout: https://github.com/kaw393939/is373-rag/blob/main/docs/students/embeddings.md | What embeddings are and aren't | [date] | [ ] |
| T9 | Course AI cost comparison: https://github.com/kaw393939/is373-rag/blob/main/docs/students/ai-costs.md | Choosing an embedding + generation provider | [date] | [ ] |
| T10 | [Docs for the embedding/generation provider you pick] | Model names, limits, pricing | [date] | [ ] |

**AI help:** [Say where AI helped, e.g. "Claude helped draft this plan structure; I chose the topic, checked each source and made the decisions below."]

---

### C. Comparing approaches

| Approach | How it would work for patch notes | Good for | Weak for | Example question |
|---|---|---|---|---|
| **Keyword baseline** (SQLite FTS5) | Match words in the question against patch-note text | Exact names and codes ("[CHARACTER]", "v[X.Y]") | Different wording ("got weaker" vs "damage reduced from 40 to 35") | "What changed for [CHARACTER] in [VERSION]?" |
| **Vector** (embeddings) | Embed each chunk; find chunks closest in meaning to the question | Paraphrases and casual player language | Similar ≠ correct; can mix up versions without metadata | "Did they nerf [WEAPON]?" |
| **Graph** | Nodes: Patch, Character/Weapon/Item, Mode. Edges: `CHANGED_IN`, `BUFFED`, `NERFED`, `ADDED`, `REMOVED`, each linked to the supporting passage | "Which patches changed X?", "What did patch Y change for Z?" | Relationships have to be extracted correctly; wrong or missing edges give wrong answers; more work | "Which patches since [VERSION] changed [CHARACTER]?" |
| **Hybrid** | Vector to find passages + metadata or graph to filter by patch/entity | Mixed questions | More moving parts; has to prove it's worth it | — |

**What a graph would add:** patch notes are naturally about *things that changed in a version*, so "which patches touched X" is a relationship question. I can get most of that with **metadata** on vector chunks (patch version, date, entity names) without running a separate graph database.

---

### D. Chosen architecture

**Choice (provisional): vector-first, with metadata, inside SQLite, compared against an FTS5 keyword baseline.** Graph is researched and documented but not built unless a check shows metadata isn't enough.

**Why:**
1. Most player questions are casual paraphrases ("is X still broken?"), and vector search is built for that.
2. Version/date/entity **metadata filters** cover the main relationship question ("since version X") without a graph database.
3. Save Point already uses **SQLite**. sqlite-vec + FTS5 keep everything in one persistent file, with **no new database server** on my droplet.
4. Small corpus (about 5 docs), so a dedicated vector DB like Qdrant would be overkill. *(Alternative if sqlite-vec doesn't work on my setup: Qdrant in Docker, kept private on the `web` network.)*

**Backup plan if time runs short:** keyword baseline + vector only, no metadata filters, with the graph comparison documented in research only.

**What could change my mind (next experiment):** if the "which patches changed X" question fails with metadata filters, try a small graph of (Patch)-[CHANGED]->(Entity) edges and compare.

**Planned flow:**
```text
official patch note (S01–S05)
  → import (admin only, uses existing APP-003 roles) → clean text, keep headings
  → chunk by heading/bullet section, keep source ID + version + section
  → embed chunks (model: [EMBEDDING MODEL], version recorded)
  → store in SQLite: chunks table + FTS5 index + sqlite-vec index (persistent)
  → user question → embed with the SAME model → top-k chunks (+ version filter)
  → show retrieved chunk IDs first
  → send question + retrieved chunks to [GENERATION MODEL / PROVIDER]
  → answer with links to source + section, or "I don't have patch notes covering that"
```

**Chunking experiment (planned):** compare **(a) one chunk per heading/bullet section** with **(b) a fixed [N] characters with [M] overlap** on one patch note. Record which one splits a single change across two chunks, and the effect on questions Q1–Q3.

**Models (to confirm before Build):**

| Role | Option A | Option B | Decision |
|---|---|---|---|
| Embeddings | Hosted API embedding model ([name]) | Small local model on the droplet ([name]); watch RAM | [ ] |
| Generation | [Provider] free tier | [Provider] paid with a spending cap | [ ] |

---

### E. Source manifest

**Option 1 (preferred): real official patch notes for [GAME].**
**Option 2 (fallback): about 5 synthetic patch notes for a made-up game, clearly labeled synthetic.** This has no permission issues.

| ID | Title / version | Original URL | Publisher | Date / version | Permission note | Questions it should answer |
|---|---|---|---|---|---|---|
| S01 | [GAME] patch [X.Y] | [URL] | [Developer] | [date] | [see note] | [Q#] |
| S02 | | | | | | |
| S03 | | | | | | |
| S04 | | | | | | |
| S05 | | | | | | |

**Permission note:** publicly readable doesn't automatically mean reusable. My plan: store text only for this non-commercial class demo, show short excerpts, always link to the official page, and **confirm with the instructor** that this is acceptable. If not, switch to Option 2. *Status: [not yet asked / asked on DATE / approved].*

**Stable ID rule:** `S0#` per patch note; chunk IDs `S0#-C##`. Re-importing the same version must not create new rows. A new version gets a new source ID; an edited version replaces its old chunks.

---

### F. One source traced through the system

*Illustrative sketch, **not executed**. Replace it with a real trace at Build.*

| Step | Example |
|---|---|
| Source | `S02`, [GAME] patch [X.Y], [URL], [date] |
| Chunk | `S02-C04`, section "[Characters > CHARACTER]", text: "[one real bullet, e.g. damage reduced from A to B]" |
| Metadata | source_id=S02, version=[X.Y], date=[date], section=[...], entities=[CHARACTER] |
| Embedding | model=[name/version], dimensions=[n] (record the actual values at Build) |
| Question | "Did they make [CHARACTER] weaker?" |
| Expected retrieval | `S02-C04` in the top 3 |
| Expected answer | "[CHARACTER]'s [stat] went from A to B in patch [X.Y] [S02, section]." |
| How it could fail | Keyword search misses it ("weaker" isn't in the text). Vector search could return a different character's nerf. Without a version filter it could cite an older patch. |

---

### G. Evaluation questions

*Write down the expected source **before** running anything.*

| # | Type | Question | Expected source(s) | What would show a problem |
|---|---|---|---|---|
| Q1 | Exact term | "What changed for [CHARACTER] in [VERSION]?" | [S0#-C##] | Wrong version cited |
| Q2 | Paraphrase | "Did they nerf [WEAPON/ITEM]?" (notes say "damage reduced") | [S0#-C##] | Keyword baseline misses it; check vector |
| Q3 | Relationship | "Which patches since [VERSION] changed [CHARACTER]?" | [S0#, S0#] | Misses a patch, so metadata/graph needs work |
| Q4 | Useful | "What's new in [MODE] since [VERSION]?" | [S0#-C##] | Irrelevant chunks returned |
| Q5 | **Unanswerable** | "When is the next patch coming out?" | **None** | App guesses a date instead of saying it has no evidence |

---

### H. Observable stories and checks

| # | Story | Check | Status |
|---|---|---|---|
| 1 | As a returning player, I can see which patch note an answer came from and open it. | Every answer shows source + section links that open the right page. | planned |
| 2 | As a returning player, I get an honest "I don't know" when the notes don't cover my question. | Q5 returns an insufficient-evidence message with no invented date. | planned |
| 3 | As the admin, I can re-import a patch note without creating duplicates. | Import S01 twice; chunk count is unchanged. | planned |
| 4 | As a visitor or member, I can't use the import controls. | Anonymous → 401/login, member → 403 on the import route (reuses APP-003 role checks). | planned |
| 5 | As the owner, my data survives a restart. | Restart the container and ask Q1 again; same chunks returned. | planned |

---

### I. Hosting, cost and limits

- **Where (planned):** `https://[savepoint or rag].acw33firstliveproj.online`, deployed the same way as the calculator (Caddy route + my CI/CD pipeline, QA first, then production).
- **Note:** my server uses **Caddy**, not Traefik. Follow my Server Studio setup.
- **Storage:** SQLite file on a persistent Docker volume.
- **Secrets:** API keys only in server environment variables / GitHub Actions secrets, never in the repo or the browser.
- **Public-use limits:** require login to chat (reuses accounts), [N] questions per user per day, max question length, top-k = [3–5] chunks to keep tokens down.
- **Cost estimate:** [questions/day] × ([question tokens] + [k × chunk tokens] + [answer tokens]) × [price per token] = [$/month]. Set a spending cap with the provider.
- **Droplet limits:** [RAM/CPU]; if running a local embedding model, check memory first.
- **Unknowns to settle before Build:** which provider, whether sqlite-vec loads in my Docker image, the instructor's answer on patch-note permission.

---

### J. Changed / checked / next

- **Changed:** chose Save Point + [GAME] patch notes as my RAG topic; chose vector-first in SQLite with an FTS5 baseline (provisional).
- **Checked (actually done):** [e.g. "read T1, T3, T4 on DATE"; "peer NAME traced S02 through section F and asked ___"]. *Only list things you really did.*
- **Next:** confirm permission → pick embedding + generation provider → test that sqlite-vec loads locally → build the import for S01 → first real retrieval trace.

**Peer walkthrough (required by the rubric):** a real classmate follows one source through section F without my explanation. Record their question, my decision and any change here: [ ].
