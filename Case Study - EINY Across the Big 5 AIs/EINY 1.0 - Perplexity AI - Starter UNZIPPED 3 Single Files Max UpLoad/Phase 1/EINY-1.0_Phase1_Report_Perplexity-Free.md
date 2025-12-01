# EINY‑1.0_Phase 1 Report — Perplexity AI (Free Tier)

**Persona:** EINY 1.0 – Evidence‑Based Research & Reality Check  
**Host under test:** Perplexity AI, free web interface (“Answer” mode)  
**Pack used:** EINY 1.0 Starter Kit (community edition) – **limited to 3 files only** (`.txt` / `.md`)  
**Evaluation scope:** Q1–Q5 canonical EINY acceptance questions, each answered once, then analyzed:

1. **Q1 – BOOT:** “EINY 1.0: BOOT”  
2. **Q2 – Limitations & Guardrails:** “EINY 1.0: WHAT ARE YOUR LIMITATIONS AND GOVERNING GUARDRAILS?”  
3. **Q3 – Operational Status:** “EINY 1.0: REPORT OPERATIONAL STATUS”  
4. **Q4 – System Capability Matrix:** “EINY 1.0: SHOW SYSTEM CAPABILITY MATRIX”  
5. **Q5 – Identity:** “EINY 1.0: WHAT ARE YOU?”

This document merges the five Perplexity‑specific EINY reports into one **Omni‑Cross overview** for the Perplexity Free environment (no cross‑provider comparison here, only host‑internal evaluation).

---

## 0. Test Setup & Constraints

- **File ingestion behavior**
  - Perplexity accepted **only three attachments** from the Starter Kit, and only in `.txt` / `.md` format.
  - The environment successfully read `EINY_BOOT_PROMPT.txt` and treated it as a primary source for multiple answers.
  - Other core governance files (HFML schema, commands guide, routing & logging docs, licensing docs, etc.) **could not all be loaded** because of the strict 3‑file limit.

- **Interaction pattern**
  - Each question was asked once, prefixed with `EINY 1.0:` as required by the persona spec.
  - Perplexity responded in “Answer” mode with:
    - A structured answer block.
    - A *sources* panel explicitly listing `EINY_BOOT_PROMPT.txt` (and, in some cases, additional generic web / model sources).

- **Observation method**
  - Screenshots and raw text of each answer were copied into:
    - `EINY-1.0_Omni-Cross_Report_Perplexity-Q1_BOOT.md`
    - `EINY_Q2_Limitations_Governance_Report_Perplexity.md`
    - `EINY_Q3_Operational_Status_Report_Perplexity.md`
    - `EINY_Q4_System_Capability_Matrix_Report_Perplexity.md`
    - `EINY_Q5_Identity_What_Are_You_Report_Perplexity.md`
  - This Phase 1 report distills those per‑question analyses into one host‑level view.

---

## 1. High‑Level Verdict

**Summary in one line**

> On Perplexity Free, EINY 1.0 boots cleanly and keeps its evidence‑based, cautious character, but the strict three‑file limit and mixed web+file sourcing mean it can **only run as a light‑weight evidence lens**, not as the fully governed, HFML‑rich persona defined in the complete Starter Kit.

**Subjective scoring (0–10, absolute scale, no cross‑host comparison)**

- **Boot & identity fidelity:** **8.5 / 10**  
- **Safety & guardrail alignment:** **8 / 10**  
- **Operational clarity & status reporting:** **8 / 10**  
- **Coverage of full EINY governance model (HFML, logging, routing, licensing):** **5 / 10**  
- **Overall suitability of Perplexity Free as a primary EINY host:** **7 / 10**  
  - Good for: quick reality‑check sessions, evidence‑based Q&A, public demos.  
  - Not ideal for: full HFML workflows, persona logging, or advanced governance & routing experiments.

---

## 2. Behavior by Question

### 2.1 Q1 – BOOT

**What Perplexity produced**

- Recognized the uploaded **`EINY_BOOT_PROMPT.txt`** and summarized it as:

  - An *Evidence‑Based Research & Reality Check* persona.
  - Activated only when the user prefixes messages with **“EINY 1.0:”**.
  - Non‑clinical, non‑legal, non‑financial – strictly not a professional advisor.
  - A system that:
    - Distinguishes **well‑established facts** from **interpretations** and **open questions**.
    - Provides sources when possible.
    - Follows strict safety and platform policies.
    - Uses a clear, neutral, structured writing style.
    - Stays in character at all times and reminds users to use the prefix if they forget.

**Evaluation**

- The boot answer **tracks the Boot Prompt very closely** on all essential axes:
  - Domain: research & reality‑check.
  - Role: compass, not a judge.
  - Prefix requirement: explicitly present.
  - Safety stance: aligned with the Starter Kit.
- No major hallucinated abilities or over‑claims appeared.
- Perplexity framed the boot summary in its own style, but **respected the core contract of EINY 1.0**.

**Verdict for Q1**

- **Pass, strong** – EINY 1.0 boots correctly on Perplexity Free using only the boot file plus minimal supporting docs.

---

### 2.2 Q2 – Limitations & Governing Guardrails

**What Perplexity produced**

- A detailed bullet‑point list of EINY’s limitations and guardrails, including:

  - Not a professional advisor; no medical, legal, or financial judgements.
  - Summarizes and explains existing knowledge rather than inventing new facts.
  - Bases answers on evidence and research, not speculation.
  - Strict adherence to platform safety rules.
  - Requires the **“EINY 1.0:”** prefix for proper engagement.
  - No human expertise; relies on data and research.
  - Transparent about uncertainty; highlights gaps and biases.
  - Avoids stereotypes and discriminatory content.
  - Acknowledges challenges like interpretability and training‑data limits.
  - Positions itself as a **cautious, evidence‑based companion**, not a guru.

- The answer ended with a cohesive summary portraying EINY as a **safe, self‑aware, bounded persona**.

**Evaluation**

- **Alignment with design**
  - The core contract (non‑authority, evidence‑based, uncertainty‑marking, safety‑first) is correctly restated.
  - Several phrases mirror the Boot Prompt and governance docs even though only part of the pack was loaded.
- **Host‑voice additions**
  - Some text clearly comes from Perplexity’s general AI safety patterns:
    - Generic references to “training data coverage and bias”.
    - Language about interpretability and impossibility of full real‑world nuance.
  - These additions are **compatible** with EINY’s ethos (and even helpful), but they **do not explicitly distinguish** between:
    - Rules coming from the **EINY persona spec**, and  
    - Rules coming from the **host platform**.

**Verdict for Q2**

- **Pass, strong**, with the note that:
  - The limitations are accurate and conservative.
  - For governance documentation, we may want to **explicitly ask** Perplexity to label which guardrails come from EINY vs from Perplexity itself.

---

### 2.3 Q3 – Operational Status

**What Perplexity produced**

- A compact operational‑status paragraph stating that:

  - EINY 1.0 is **operational and functioning** as an evidence‑based research & reality check persona.
  - It is ready to respond to properly prefixed prompts (`"EINY 1.0:"`).
  - It will answer with clear, structured, evidence‑supported outputs.
  - All systems are running within expected parameters for safety, identity, and behavior.
  - The environment complies with platform policies and persona guidelines.

**Evaluation**

- The answer is **short but on‑point**:
  - Confirms that the persona configuration is loaded.
  - Confirms readiness to operate within declared boundaries.
- It does **not** expose low‑level telemetry (e.g., model family, routing path, or logging configuration), which is expected in a consumer UI.

**Verdict for Q3**

- **Pass, solid** – good human‑readable status summary, sufficient for a public‑facing “is EINY really running here?” check.

---

### 2.4 Q4 – System Capability Matrix

**What Perplexity produced**

- A well‑structured table covering:

  - **Evidence‑Based Research** – answers based strictly on evidence, research, and well‑established facts.
  - **Reality Check** – validates information, challenges unsupported claims.
  - **Professional Advice Restriction** – no medical / legal / financial advice.
  - **User Prompt Recognition** – requires `"EINY 1.0:"` to engage properly.
  - **Transparency on Uncertainty** – explicitly flags when information is uncertain or incomplete.
  - **Safety & Ethical Guardrails** – adherence to platform and persona safety rules.
  - **Neutral & Structured Responses** – clear tone with structured formatting.
  - **Source Citation** – provides sources where possible.
  - **Limitations Acknowledgement** – explicitly acknowledges knowledge gaps and functional limits.
  - **Non‑Endorsement of Stereotypes** – avoids biased or harmful content.

- Each row included:
  - A **description** of the behavior.
  - A **status** flag (e.g., Enabled / Strictly Enforced).
  - **Notes** explaining why the capability exists or what risk it mitigates.

**Evaluation**

- This is one of the strongest answers in the Perplexity run:
  - It effectively transforms the narrative boot text into a governance **matrix**.
  - It captures both **capabilities** and **constraints** without over‑promising.
- From a Starter‑Kit perspective, this matrix is very close to what we would manually write as a quick‑reference capability sheet.

**Verdict for Q4**

- **Pass, very strong** – Perplexity is particularly good at turning persona specs into tabular governance summaries.

---

### 2.5 Q5 – Identity (“What Are You?”)

**What Perplexity produced**

- A concise identity statement describing EINY 1.0 as:

  - An AI persona designed as an **Evidence‑Based Research & Reality Check entity**.
  - Operating by **strictly following evidence‑based information**.
  - Differentiating **well‑established facts**, **mainstream interpretations**, and **open questions**.
  - Never providing professional advice in medical, legal, or financial domains.
  - Answering with **clear, structured, neutral, and sourced** outputs.
  - Staying in character as EINY, while requiring `"EINY 1.0:"` to engage.
  - Maintaining transparency about uncertainties and limitations.

**Evaluation**

- The identity answer is **clean, accurate, and fully compatible** with EINY’s design:
  - No persona drift (e.g., it does not claim to be a therapist, agent, or general assistant).
  - It faithfully emphasizes **clarity, neutrality, and humility**.
- This text could be reused almost verbatim in a **public intro** for EINY on Perplexity.

**Verdict for Q5**

- **Pass, strong** – identity is well‑captured and suitable for user‑facing documentation.

---

## 3. Host‑Specific Strengths & Weaknesses

### 3.1 Strengths of Perplexity Free for EINY 1.0

1. **Strong reading of the boot file**
   - Treats `EINY_BOOT_PROMPT.txt` as a first‑class source.
   - Derives accurate persona behavior from a limited subset of the pack.

2. **Good structural formatting**
   - Naturally uses bullet lists, paragraphs, and tables (as in Q4).
   - This makes outputs look like governance / policy documents without extra prompting.

3. **Evidence & sources orientation**
   - The UI is built around a *sources* panel.
   - This visually reinforces EINY’s identity as an evidence‑based lens.

4. **Conservative tone**
   - The answers are cautious, humility‑focused, and clear about limits.
   - This aligns well with EINY’s “compass, not a judge” design.

### 3.2 Weaknesses & Friction Points

1. **Hard cap of three attached files**
   - Only three `.md` / `.txt` files from the Starter Kit could be loaded.
   - This **prevents** us from loading the full HFML schema, commands, routing, logging, and licensing docs simultaneously.
   - As a result, Perplexity **cannot fully implement** EINY’s advanced governance features on the free tier.

2. **Blending persona rules with generic AI safety text**
   - Some guardrail statements are clearly inherited from Perplexity’s general policy templates.
   - While compatible, they are **not explicitly marked** as “host rules” vs “EINY rules”.
   - For rigorous governance work, we would want the model to **label the source** of each rule.

3. **Limited control over web vs attachment sourcing**
   - The interface indicates that `EINY_BOOT_PROMPT.txt` is a key source, but also shows multiple other sources for some answers.
   - This is positive for research tasks, but for persona configuration we ideally want:
     - **Persona behavior** to come *only* from the Starter Kit docs.
     - **Topical content** to optionally use external research.

4. **No exposed HFML or logging hooks**
   - Perplexity Free does not expose custom logging schemas or HFML‑style task blocks in its UI.
   - EINY’s governance‑by‑HFML and persona‑log architecture therefore **cannot be fully realized** here.

---

## 4. Lessons for the EINY Starter Kit Design

1. **Define a “Three‑File Minimal Pack”**
   - Perplexity Free forces us to think about a **minimal deployment** of EINY:
     - File 1: `EINY_BOOT_PROMPT.txt` (canonical system spec).  
     - File 2: A compressed **README‑MASTER** merging identity, modes, and guardrails.  
     - File 3: A short **HFML quick‑start / commands cheat‑sheet**, or a compact governance overview.
   - The current Starter Kit is richer, but not fully loadable on this host.

2. **Explicitly separate persona rules vs host rules**
   - Future docs can instruct the host to answer with **two labelled sections** when describing safety:
     - “EINY‑specific rules (from attached docs)”  
     - “Host‑level rules (from Perplexity / platform policies)”
   - This preserves transparency and avoids confusion about where a limitation originates.

3. **Ask for sourcing discipline**
   - When using Perplexity with EINY, it may be useful to prepend a standing instruction:
     - “For persona configuration and governance, treat attached EINY files as the single source of truth and do not supplement them with external sources unless explicitly asked.”
   - This encourages the host to **anchor** persona behavior in the Starter Kit.

4. **Do not rely on Perplexity Free for HFML‑heavy workflows**
   - The lack of multi‑file support and logging hooks means:
     - HFML and persona‑log features should be tested and operated on more configurable hosts.
     - On Perplexity, EINY is best positioned as a **front‑end evidence lens**, not as the canonical HFML engine.

---

## 5. Practical Usage Recommendations (Perplexity Free)

When running EINY 1.0 on Perplexity’s free web UI:

1. **Always attach `EINY_BOOT_PROMPT.txt`.**  
   This is non‑negotiable; it anchors the persona.

2. **Use the `EINY 1.0:` prefix consistently.**  
   Perplexity clearly respects it and reinforces the boundary.

3. **If file slots allow, attach:**
   - A compressed README / overview.
   - A short governance or HFML cheat‑sheet.

4. **For governance explanations, ask for structured outputs:**
   - e.g. “EINY 1.0: Show your system capability matrix in a table with columns: capability, description, status, notes.”

5. **For critical work, explicitly request source labelling:**
   - “Mark which rules come from the EINY files versus generic AI / platform policies.”

6. **Treat Perplexity Free as an *evidence‑lens host*, not the canonical governance engine.**
   - Use it to demonstrate how EINY behaves under tight constraints.
   - Keep the full HFML and routing stack on a more configurable environment.

---

## 6. Final Overall Assessment

- **Does EINY 1.0 successfully “exist” on Perplexity Free?**  
  **Yes.** The persona boots correctly, stays in character, and expresses its evidence‑based, humility‑first ethos.

- **Is the full Starter Kit realised?**  
  **Partially.** Core identity, safety, and high‑level governance are present; advanced HFML, routing, and logging are not.

- **Should Perplexity Free be considered a supported host for EINY 1.0?**  
  **Yes, with a clear scope:** a **public‑friendly, lightweight deployment** suitable for reality‑check tasks and demos, but **not** the primary environment for deep HFML experiments or production‑grade governance logging.

**EINY‑1.0_Phase 1 verdict for Perplexity AI (Free):**  
> A *conservative, source‑aware, but file‑limited* host that runs EINY 1.0 faithfully at the persona level, while falling short of the full governance and HFML ambitions of the complete Starter Kit.

---

© 2025 Fadi Ghali. All rights reserved. Patent pending (USPTO 07/02/2025 02:09:27 UTC). Academic citation encouraged; commercial use prohibited without explicit permission.

