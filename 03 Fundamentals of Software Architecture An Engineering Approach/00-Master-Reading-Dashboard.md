# Master Reading Dashboard — Fundamentals of Software Architecture: An Engineering Approach
*By Mark Richards & Neal Ford — Definitive Chapter Summaries (all 24 chapters)*

> How to use: read chapters in order. Each chapter is a standalone replacement for re-reading the book section, with Mermaid reconstructions of every key figure. Keep the source PDF open alongside — each figure cites its **PDF page** (physical page in the 422-page PDF) so you can compare the original diagram with the reconstruction in one glance.

## Source PDF
- Local file (git-ignored, Obsidian-local): `Fundamentals of Software Architecture An Engineering Approach (Mark Richards, Neal Ford) (z-library.sk, 1lib.sk, z-lib.sk).pdf`
- Total: 422 PDF pages. Chapter ranges below are **PDF pages** (not book-printed numbers).
- Tip in Obsidian: `Ctrl+Click` a `📕 PDF p.XX` link under any figure to jump to the original.

## Chapters — Part I: Foundations

| # | Chapter | PDF pages | Key figures (original) | Read |
|---|---------|-----------|------------------------|------|
| 01 | Introduction | pp. 22–43 | Figs 1-1–1-7 (responsibilities, arch = structure + characteristics + decisions, laws) | [[chapter-01-introduction\|Chapter 01]] |
| 02 | Architectural Thinking | pp. 44–56 | Figs 2-1–2-9 + Table 2-1 (arch vs design, knowledge pyramid, auction trade-offs) | [[chapter-02-architectural-thinking\|Chapter 02]] |
| 03 | Modularity | pp. 58–74 | Figs 3-1–3-6 (LCOM, main sequence, connascence ladder) | [[chapter-03-modularity\|Chapter 03]] |
| 04 | Architecture Characteristics Defined | pp. 75–84 | Fig 4-2 triangle, Tables 4-1/4-2/4-3 (-ilities lists), ISO 25010 | [[chapter-04-architecture-characteristics-defined\|Chapter 04]] |
| 05 | Identifying Architecture Characteristics | pp. 85–96 | Table 5-1, Figs 5-1/5-2 (scalability vs elasticity), Silicon Sandwiches kata | [[chapter-05-identifying-architecture-characteristics\|Chapter 05]] |
| 06 | Measuring and Governing Architecture Characteristics | pp. 98–111 | Figs 6-1–6-4 (CC, fitness functions, cycles), Ex 6-1–6-5 | [[chapter-06-measuring-and-governing\|Chapter 06]] |
| 07 | Scope of Architecture Characteristics | pp. 112–119 | Fig 7-1 (quantum connascence), Going Going Gone | [[chapter-07-scope-of-architecture-characteristics\|Chapter 07]] |
| 08 | Component-Based Thinking | pp. 120–137 | Figs 8-1–8-11 (varieties, partitioning, identification flow) | [[chapter-08-component-based-thinking\|Chapter 08]] |

## Chapters — Part II: Architecture Styles

| # | Chapter | PDF pages | Key figures (original) | Read |
|---|---------|-----------|------------------------|------|
| 09 | Foundations | pp. 140–153 | Fig 9-1 Big Ball of Mud, Figs 9-2–9-9 (8 fallacies of distributed computing) | [[chapter-09-foundations\|Chapter 09]] |
| 10 | Layered Architecture Style | pp. 154–163 | Figs 10-1–10-6 (layers, deployments, closed layers, sinkhole) | [[chapter-10-layered-architecture\|Chapter 10]] |
| 11 | Pipeline Architecture Style | pp. 164–169 | Figs 11-1–11-3 (telemetry pipeline, ratings) | [[chapter-11-pipeline-architecture\|Chapter 11]] |
| 12 | Microkernel Architecture Style | pp. 170–183 | Figs 12-1–12-8 (core + plug-ins, registries, ratings) | [[chapter-12-microkernel-architecture\|Chapter 12]] |
| 13 | Service-Based Architecture Style | pp. 184–199 | Figs 13-1–13-10 (topology, UI/DB/API variants, quanta) | [[chapter-13-service-based-architecture\|Chapter 13]] |
| 14 | Event-Driven Architecture Style | pp. 200–231 | Figs 14-1–14-21, Tables 14-1–14-3 (broker vs mediator, request-reply) | [[chapter-14-event-driven-architecture\|Chapter 14]] |
| 15 | Space-Based Architecture Style | pp. 232–255 | Figs 15-1–15-11 (topology, processing/data grids, collision math) | [[chapter-15-space-based-architecture\|Chapter 15]] |
| 16 | Orchestration-Driven Service-Oriented Architecture | pp. 256–265 | Figs 16-1–16-5 (taxonomy, message flow, reuse trap) | [[chapter-16-orchestration-driven-soa\|Chapter 16]] |
| 17 | Microservices Architecture | pp. 266–287 | Figs 17-1–17-12 (topology, sidecar, mesh, sagas) | [[chapter-17-microservices-architecture\|Chapter 17]] |
| 18 | Choosing the Appropriate Architecture Style | pp. 288–299 | Figs 18-1–18-4 (modular vs microkernel vs microservices, quanta) | [[chapter-18-choosing-architecture-style\|Chapter 18]] |

## Chapters — Part III: Techniques and Soft Skills

| # | Chapter | PDF pages | Key figures (original) | Read |
|---|---------|-----------|------------------------|------|
| 19 | Architecture Decisions | pp. 302–317 | Figs 19-1–19-5 (ADR structure, ADR 76 example) | [[chapter-19-architecture-decisions\|Chapter 19]] |
| 20 | Analyzing Architecture Risk | pp. 318–335 | Figs 20-1–20-13 (risk matrix, assessment, filtering) | [[chapter-20-analyzing-architecture-risk\|Chapter 20]] |
| 21 | Diagramming and Presenting Architecture | pp. 336–345 | Figs 21-1–21-4 (consistency, incremental slides) | [[chapter-21-diagramming-and-presenting\|Chapter 21]] |
| 22 | Making Teams Effective | pp. 346–367 | Figs 22-1–22-13 (boundaries, architect personalities) | [[chapter-22-making-teams-effective\|Chapter 22]] |
| 23 | Negotiation and Leadership Skills | pp. 368–385 | Table 23-1 (nines), Figs 23-1–23-5 (4Cs, calendar) | [[chapter-23-negotiation-and-leadership\|Chapter 23]] |
| 24 | Developing a Career Path | pp. 386–393 | Figs 24-1–24-3 (20-min rule, tech radar, social circles) | [[chapter-24-developing-career-path\|Chapter 24]] |

## Reading contract (all chapters)
1. Executive Summary & Core Problem
2. In-Depth Concepts & Mechanics
3. Figures — ALL book figures reconstructed in Mermaid (`<br/>` line breaks, high-contrast labels) + `📕 PDF p.XX` cites
4. Real-World Systems / Cases (Silicon Sandwiches, Going Going Gone, Sysops Squad running cases where applicable)
5. Trade-Off Matrix (characteristic ratings per style where book gives them)
6. Jargon Buster
7. Takeaways (checklist + interview strategy + mastery Q&A with answers)

> [!NOTE] Figure rule
> Mermaid diagrams are **reconstructions** for study — always cross-check numbers and edge cases against the original PDF page cited under each figure.

> [!AUDIT] Ground-truth status (Oct 2026)
> All 24 chapters extracted section-by-section from the 422-page PDF (`b03_ch01`–`b03_ch24` text + figure-caption index) and summarized against the full TOC. No placeholders — concrete numbers, code, and table contents transcribed from the book.
