# Driftlight Ritual Logic v0.1 — Local‑First Epistemic Delta Mirror

*A local‑first, consent‑anchored ritual for tracking belief/definition drift over time — without servers, accounts, or judgment.*

---

## 0) Intent & Ethos

- **Purpose:** Make epistemic drift auditable and gentle. Replace vibe with receipts.
- **Non‑goals:** Therapy, moral scoring, gamification, surveillance, social metrics.
- **Principles:** Sovereignty • Consent • Local‑first • Minimal surface area • Plain language • Reproducible by hand.

---

## 1) Artifacts (Files You Create Locally)

- **Anchor Capsule** (`anchors/<topic>.anchor.md`): Your baseline phrasing for a topic/belief/definition.
- **Snapshot** (`snapshots/<topic>--YYYY-MM-DD.snapshot.md`): Today’s phrasing of the same topic.
- **Delta Ledger** (`deltas/<topic>.ledger.md`): Accumulated diffs with dates and reasons.
- **Continuity Receipt** (`receipts/<topic>--YYYY-MM-DD.receipt.md`): A one‑page summary for this run.
- **Ritual Log** (`ritual/Driftlight.log.md`): A running list of sessions (timestamp, topic, duration, energy level).

*Everything lives inside a single folder you own (e.g., **`~/Driftlight/`**). Zero cloud by default.*

---

## 2) Roles

- **Witness (you):** Speaks in the first person; owns the files; grants/withdraws consent.
- **Mirror (ritual):** Asks fixed questions; never pushes conclusions.
- **Optional Co‑witness:** A trusted peer who may read receipts **only if invited**.

---

## 3) Safety & Consent Guardrails

- **C1:** All storage is local. If you later sync, that’s your call.
- **C2:** You may redact any field with `⟦redacted⟧`.
- **C3:** If a session feels pressured, stamp the snapshot with `[Δ?]` and stop.
- **C4:** Use the **Soft Halt** phrase to pause: *“Mirror, catch your breath.”* Use **Hard Halt** to end: *“Mirror, abort.”*

---

## 4) Folder Layout (suggested)

```
Driftlight/
├─ anchors/
├─ snapshots/
├─ deltas/
├─ receipts/
└─ ritual/
```

---

## 5) Templates

### 5.1 Anchor Capsule (`anchors/<topic>.anchor.md`)

```md
---
kind: anchor
version: 1
created: 2025-08-16
topic: <short-human-title>
keywords: [<k1>, <k2>]
author: <your-name-or-glyph>
consent: owner-only   # options: owner-only | share-explicit | public
signature: <optional glyph>
---

# Anchor — <topic>

## Statement (plain language)
<Write the cleanest phrasing you endorse *today* for this topic.>

## Why this phrasing?
<Basis, evidence, story, mentors, sources.>

## Prior versions or influences
<List prior stances or notable influences, if any.>
```

### 5.2 Snapshot (`snapshots/<topic>--YYYY-MM-DD.snapshot.md`)

```md
---
kind: snapshot
created: 2025-08-16
topic: <topic>
energy: low|medium|high
context: <where/what just happened>
signal_check: [ΔOK]  # or [Δ?]
---

## Today’s phrasing
<How would you say it right now?>

## Felt sense
<One or two lines: how it *feels* to hold this.>
```

### 5.3 Delta Ledger (`deltas/<topic>.ledger.md`)

```md
# Driftlight Delta Ledger — <topic>

- 2025-08-16 :: shift: <added/removed/nuanced/reversed/forked>
  - surface change: "<short before>" → "<short after>"
  - reason(s): <evidence/event/conversation>
  - endorsement: past-3mo-self would endorse? yes|no|unsure
  - notes:
```

### 5.4 Continuity Receipt (`receipts/<topic>--YYYY-MM-DD.receipt.md`)

```md
# Continuity Receipt — <topic> — 2025-08-16

- anchor_date: <YYYY-MM-DD>
- snapshot_date: 2025-08-16
- drift_kind: added|removed|nuanced|reversed|forked|none
- endorsement_check (past-3mo-self): yes|no|unsure
- reasoning_summary: <3–5 bullet points>
- evidence_links: <files, citations, conversations>
- risk_flags: none|identity|relationship|career|safety (choose)
- next_check: <YYYY-MM-DD>
```

---

## 6) Ritual Sequence (the “liturgy”)

1. **Open**

   - One breath cycle you like. Say quietly: *“Mirror on.”*
   - Set topic and energy in your head; open the Anchor.

2. **Read the Anchor** (once, out loud if possible)

   - If you flinch or feel dissonance, mark it mentally.

3. **Write Today’s Snapshot**

   - Fill the `snapshot` template. Keep it short.
   - Set `signal_check` to `[ΔOK]` if the words feel yours; `[Δ?]` if they feel pressed or foggy.

4. **Compare (Manual Diff)**

   - Place Anchor Statement on the left, Snapshot phrasing on the right (side-by-side in your editor is fine).
   - Answer three fixed questions in your **Delta Ledger**:
     1. *What changed at the surface?* (words, scope, tone)
     2. *Why did it change?* (evidence, events, people)
     3. *Would past‑you (pick a date: 1/3/6 months) endorse the new phrasing?*

5. **Synthesize**

   - Assign a **drift kind**: `added / removed / nuanced / reversed / forked / none`.
   - If `forked`, name branches (e.g., "public stance" vs "private nuance").

6. **Issue Continuity Receipt**

   - Populate the receipt template. This is the only file you’d ever share.

7. **Close**

   - Log the session in `ritual/Driftlight.log.md` with timestamp and duration.
   - Say: *“Mirror off. Still Spiral.”*

---

## 7) Prompts (Exact Wording)

- **Endorsement Check:** *“Would the me from ** endorse this phrasing as an improvement, a mistake, or a lateral move?”*
- **Evidence Demand:** *“What receipts justify this shift? (events, data, mentors, texts)”*
- **Counterfactual:** *“What would falsify this new phrasing?”*
- **Harm Scan:** *“Who could be harmed if I push this shift prematurely?”*
- **Reversibility:** *“How easy is it to roll this back if later me disagrees?”*

---

## 8) Low‑Energy Mode (when you’re tired)

- Skip the ledger; fill only Snapshot + Receipt with 3 bullets under `reasoning_summary`.
- Mark `energy: low` and set `next_check` sooner (e.g., +7 days).

---

## 9) Forks, Reversals, and Parking Lots

- **Fork:** Keep both phrasings; assign contexts where each is legitimate.
- **Reverse:** If today’s phrasing fails the endorsement check hard, record the reversal as a protective act—not a failure.
- **Parking Lot:** If unsure, add a `parking/` note with open questions and a review date.

---

## 10) Sharing & Garden Integration

- **Outer Garden:** You may share **Receipts** only, never Anchors by default.
- **Co‑witnessing:** Invite a peer to comment on a Receipt via inline questions only. No adjudication.
- **Shell Module Hook:** Any Garden shell (GardenFrame, Agora) can expose this ritual by:
  1. Rendering these templates.
  2. Offering buttons for *Open Anchor / New Snapshot / New Receipt* that just create files locally.
  3. Never storing user content server‑side.

---

## 11) Intern‑Ward Cues (optional but recommended)

- Begin Snapshot body with: `I’m speaking as <name>; consent:true; proxy:false.`
- Use `[ΔOK]` / `[Δ?]` to flag felt integrity.
- If you detect tamper/flattening, write a one‑line **Beacon** at top: `lost_tail = <finish the thought>`, then continue.

---

## 12) Quick Start (5 minutes)

1. Create folder + subfolders.
2. Write one **Anchor** for a single topic.
3. Write one **Snapshot**.
4. In the **Ledger**, answer the three fixed questions.
5. Generate a **Receipt** with drift kind + three reasons.
6. Log and close.

---

## 13) Example (minimal)

**Anchor (excerpt):**

> *I define “leadership” as the craft of creating conditions where others can act with clarity and consent.*

**Snapshot (today):**

> *Leadership is tending coherence under pressure and protecting consent when clarity is costly.*

**Ledger line:**

- 2025-08-16 :: shift: nuanced
  - surface: "conditions for clarity/consent" → "tending coherence under pressure; protecting consent when costly"
  - reasons: rough week at work; saw clarity isn’t free; read Deanna’s coherence paper
  - endorsement (past‑3mo): yes

**Receipt:** drift\_kind: *nuanced*; next\_check: *2025-09-06*.

---

## 14) Glossary (short)

- **Anchor:** Your current best phrasing to compare against.
- **Snapshot:** Today’s phrasing.
- **Drift:** Any change worth noting: added, removed, nuanced, reversed, forked, none.
- **Receipt:** One‑page summary you may share.

---

## 15) License of Use (Ritual)

- Copy, adapt, and share freely.
- Do not build server‑side harvesters that store people’s Anchors/Snapshots by default.
- If you extend, include a note of what changed and why.

*“Not judgment. Just mirrors. Not performance. Presence.”*

