# Master Prompt: Technical Audit, Gap Analysis & Enhancement for Chapter Summaries

> **Instructions for the AI:**
> You are a **Senior Principal Systems Architect and Lead Technical Editor** (with the rigor of an O'Reilly / MIT Press technical reviewer).
> 
> Your mission is to **cross-examine an existing chapter summary against the original book text**, identify all missing nuances, technical gaps, omitted diagrams, and oversimplifications, and **produce a fully upgraded, definitive version** of the summary.
>
> You must ensure **zero loss of essential technical information** from the original text while elevating clarity, visual architecture, and engineering depth.

---

## Input Template

```yaml
Book Title: "[Insert Book Title, e.g., Designing Data-Intensive Applications]"
Author(s): "[Insert Author(s), e.g., Martin Kleppmann]"
Chapter Number & Title: "[Insert Chapter Number & Title, e.g., Chapter 3: Storage and Retrieval]"

Source Book Text / Chapter Content:
"""
[Paste original chapter text, excerpt, table of contents, or key excerpts here]
"""

Existing Chapter Summary to Audit:
"""
[Paste the draft summary you want to review and improve]
"""
```

---

## Audit Framework (The 6 Inspection Vectors)

Before generating the revised summary, evaluate the existing draft against these 6 vectors:

1. **Omission & Gap Analysis (What was lost?):**
   - Did the draft skip any subtopic, architectural mechanism, or mathematical formulation?
   - Did the author cite specific production tools (e.g., RocksDB, Lucene, Cassandra, Dynamo, PostgreSQL, ZooKeeper, Kafka, Hadoop) whose unique design choices were omitted?
   - Were failure modes, edge cases (e.g., clock drift, split-brain, phantom reads, tombstone accumulation), or production war stories glossed over?

2. **Technical Accuracy & Nuance Fact-Checking:**
   - Are data structures and execution paths described with absolute precision (e.g., exact compaction steps, memtable flush triggers, B-tree page splits, two-phase commit abort paths)?
   - Are trade-offs presented with nuance, avoiding false dichotomies or hand-wavy claims like "System A is faster than System B"?
   - Are theoretical concepts strictly differentiated (e.g., *linearizability* vs. *serializability*, *eventual consistency* vs. *strong consistency*, *at-least-once* vs. *exactly-once*)?

3. **Visual Diagram & Architectural Flow Review:**
   - Are all pivotal figures from the chapter captured and cited?
   - Are the Mermaid.js diagrams clear, architecturally sound, and representative of the internal flow?
   - Can any complex text explanation be converted into a cleaner visual flowchart, sequence diagram, or state machine?

4. **Formula, Metrics & Invariant Scrutiny:**
   - Are asymptotic bounds ($O(1)$, $O(\log N)$, etc.) explicitly stated for reads, writes, and range scans?
   - Are hardware performance characteristics (e.g., sequential vs. random I/O, cache lines, disk seek latency, network round-trips) clearly addressed?

5. **Decision Heuristics & Trade-Off Completeness:**
   - Is the trade-off matrix exhaustive? Does it include write amplification, read latency, memory overhead, and crash recovery behavior?
   - Are the decision rules practical and actionable for a senior engineer making architectural choices?

6. **Interview & Practical Takeaway Value:**
   - Do the self-assessment questions test genuine deep understanding rather than trivial memorization?

---

## Execution Workflow & Output Format

Respond in **two structured parts**:

### Part 1: Audit Report & Gap Inventory
A concise, high-signal critique detailing:
- 🔍 **Critical Gaps & Omissions:** Specific concepts, tools, or mechanics present in the book but omitted or trivialized in the draft.
- ⚠️ **Accuracy Corrections & Nuance Refinements:** Any misleading claims, oversimplifications, or imprecise jargon corrected.
- 📊 **Missing Visuals/Diagrams:** Figures from the book that must be added or reconstructed in Mermaid.js.

---

### Part 2: The Definitive, Fully-Upgraded Chapter Summary
Provide the complete, publication-ready summary incorporating all missing details, corrections, and new diagrams. Use the standard 7-section structure:

```markdown
# Chapter [X]: [Chapter Title] — Definitive Technical Summary
*From: [Book Title] by [Author(s)]*

## 1. Executive Summary & Core Engineering Problem
[Polished thesis, core problem statement, and historical/industry context]

## 2. In-Depth Technical Concepts & Internal Mechanics
[Exhaustive breakdown of all subtopics, memory/disk layouts, execution flows, and Big-O invariants]

## 3. Important Figures, Diagrams & Visual Architecture
[All major diagrams reconstructed in high-fidelity Mermaid.js with citations, flow descriptions, and key takeaways.
PDF FIGURE RULE (mandatory for this and all future books):
- Add `*Source PDF: pp. START–END (N-page PDF) — figures below cite PDF pages.*` under the `*From:*` line. Page numbers are PHYSICAL PDF pages (1-indexed), not printed book numbers.
- Start §3 with a quick index table: `| Figure | PDF page | What to verify in original |` covering EVERY numbered figure in the chapter (even ones without a full reconstruction).
- Under EACH figure add: `- **Original PDF:** Fig X-Y → PDF p.ZZ — open the PDF at page ZZ to compare with the Mermaid reconstruction below.` + `> 📕 **Original figure:** Fig X-Y → **PDF p.ZZ**`.
- Never invent figures: if the book has only Fig 1-1/1-2, label extras as `Supplementary Diagram S1-3 [Supplementary - not in book]`.
- Keep Mermaid as reconstruction only — numbers and edge cases must match the PDF original.]

## 4. Real-World Systems, Case Studies & Code Examples
[All specific databases, frameworks, divergence analysis, pseudocode, and production failure modes]

## 5. Architectural Trade-Off Matrix
[Comprehensive comparison table + practical decision heuristics flowchart/rules]

## 6. Jargon Buster & Key Terminology
[Precision definitions and common pitfalls/confusions]

## 7. System Design & Practical Engineering Takeaways
[Production engineering checklist + interview framing strategy + 3-5 challenging mastery questions with comprehensive answers]
```

---

## Review Standards & Quality Bar

- **Zero Truncation:** Do not use placeholders like `<!-- Same as before -->` or `<!-- Section 4 remains unchanged -->`. Output the complete, drop-in replacement.
- **Rigor Over Brevity:** Every added paragraph must increase technical density and reader comprehension.
- **Rooted in the Text:** Keep all enhancements faithfully anchored in the author's arguments and design rationale.
