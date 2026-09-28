# Books Summary

In-depth, publication-grade technical compendiums of foundational software engineering books. Focused on storage internals, distributed systems algorithms, quantitative trade-offs, and Staff+ (L6/L7) system design preparation.

---

## 📚 Completed Books

### 01. Designing Data-Intensive Applications (2nd Edition)
**Authors:** Martin Kleppmann & Chris Riccomini  
**Word Count / Depth:** 757+ KB of rigorous technical analysis, 100+ Mermaid architectural diagrams, production-grade Python implementations, and quantitative derivations.

| Chapter | Title | Key Mechanics & Algorithms | Reading Link |
| :---: | :--- | :--- | :---: |
| **01** | Trade-Offs in Data Systems Architecture | Reliability, Scalability, Maintainability, Fan-out architecture | [Read Chapter 01](./01 Designing Data-Intensive Applications/chapter-01-trade-offs-in-data-systems-architecture.md) |
| **02** | Defining Nonfunctional Requirements | Latency percentiles (p95, p99, p99.9), SLO/SLA/SLI, Head-of-line blocking | [Read Chapter 02](./01 Designing Data-Intensive Applications/chapter-02-defining-nonfunctional-requirements.md) |
| **03** | Data Models and Query Languages | Relational vs Document vs Graph, Cypher, SPARQL, MapReduce queries | [Read Chapter 03](./01 Designing Data-Intensive Applications/chapter-03-data-models-and-query-languages.md) |
| **04** | Storage and Retrieval | Bitcask, SSTables, LSM-trees, Bloom filters, B-Trees, Columnar, Vector/HNSW | [Read Chapter 04](./01 Designing Data-Intensive Applications/chapter-04-storage-and-retrieval.md) |
| **05** | Encoding and Evolution | Protobuf Varints/ZigZag, Avro Schema Resolution, Schema Registries, Temporal | [Read Chapter 05](./01 Designing Data-Intensive Applications/chapter-05-encoding-and-evolution.md) |
| **06** | Replication | Single-Leader failover, Replication lag anomalies, Multi-Leader CRDTs, Quorums | [Read Chapter 06](./01 Designing Data-Intensive Applications/chapter-06-replication.md) |
| **07** | Sharding | Hash vs Range partitioning, Consistent Hashing/vnodes, Scatter-Gather routing | [Read Chapter 07](./01 Designing Data-Intensive Applications/chapter-07-sharding.md) |
| **08** | Transactions | ACID realities, MVCC Snapshot Isolation, Lost Updates, Write Skew, SSI, 2PC | [Read Chapter 08](./01 Designing Data-Intensive Applications/chapter-08-transactions.md) |
| **09** | The Trouble with Distributed Systems | Partial failures, Physical clock drift, Google TrueTime, Monotonic fencing | [Read Chapter 09](./01 Designing Data-Intensive Applications/chapter-09-the-trouble-with-distributed-systems.md) |
| **10** | Consistency and Consensus | Linearizability, Cross-channel races, CAP/PACELC, Total Order, Raft/Paxos | [Read Chapter 10](./01 Designing Data-Intensive Applications/chapter-10-consistency-and-consensus.md) |
| **11** | Batch Processing | Unix philosophy, MapReduce shuffle, Spark RDD lineage, Sort-Merge joins | [Read Chapter 11](./01 Designing Data-Intensive Applications/chapter-11-batch-processing.md) |
| **12** | Stream Processing | Log brokers (Kafka), Debezium CDC, Stream-Table duality, Watermarks, Chandy-Lamport | [Read Chapter 12](./01 Designing Data-Intensive Applications/chapter-12-stream-processing.md) |
| **13** | A Philosophy of Streaming Systems | Unbundling databases, End-to-end correctness, Timeliness vs Integrity, Merkle audit | [Read Chapter 13](./01 Designing Data-Intensive Applications/chapter-13-a-philosophy-of-streaming-systems.md) |
| **14** | Doing the Right Thing | Algorithmic bias, Feedback loops, Surveillance capitalism, Crypto-shredding, DP | [Read Chapter 14](./01 Designing Data-Intensive Applications/chapter-14-doing-the-right-thing.md) |

---

## 🎨 Obsidian Reading Experience

> Calm, eye-friendly, no clutter — designed so long reads don't tire the eyes (چشم‌ها را اذیت نمی‌کند، مرتب و بدون شلوغ‌کاری).

This repository includes a custom calm-minimal Obsidian reading design in `.obsidian/snippets/perfect-reading-theme.css` (v2):
- **Eye-Comfort Palette**: Deep midnight slate for Dark Mode, warm paper for Light Mode. Solid headings (no gradient glare), single-accent hierarchy, flat tables and blockquotes.
- **Ergonomic Typography**: `Plus Jakarta Sans`, `Vazirmatn` (Persian/RTL-ready), `JetBrains Mono`. Optimal `860px` line length, `1.8` line height, generous paragraph rhythm.
- **Calm Markdown Elements**: Soft tables (no sticky jump), plain code blocks, quiet Mermaid containers, visible focus rings, `prefers-reduced-motion` + print styles.
- **Figure-Aware**: Every figure cites its source **PDF page** (`📕 PDF p.XX`) — keep the PDF open alongside Obsidian to compare originals with Mermaid reconstructions.
- **Zero Configuration Required**: Open this repository as an Obsidian Vault, and the theme is automatically loaded and applied.

---

## 📖 Chapter Architecture Standard

Every chapter compendium adheres strictly to this 7-section contract (see `CHAPTER_SUMMARY_PROMPT.md` / `CHAPTER_REVIEW_AND_IMPROVEMENT_PROMPT.md`):
1. **Executive Summary & Core Engineering Problem**: Thesis, breaking example, historical context.
2. **In-Depth Technical Concepts & Internal Mechanics**: Theory, numbered data paths, byte layouts, Big-O, pseudocode, edge + failure modes.
3. **Important Figures, Diagrams & Visual Architecture**: Quick index of **all original book figures with PDF pages** (`📕 PDF p.XX`), then per-figure Mermaid reconstructions with reference, flow, diagram, takeaway. Supplementary diagrams are labeled `[Supplementary - not in book]`.
4. **Real-World Systems, Case Studies & Code Examples**: Implementations, divergences, error-path code, war stories.
5. **Architectural Trade-Off Matrix**: `| Approach | Read | Write | Storage | Recovery | Best When | Worst When |` + decision heuristics.
6. **Jargon Buster & Key Terminology**: Plain-English + precise + confused-with (8+ terms).
7. **System Design & Practical Engineering Takeaways**: Checklist, interview framing, 3 mastery Q&A with numbers.

Start here: [Master Reading Dashboard](./01%20Designing%20Data-Intensive%20Applications/00-Master-Reading-Dashboard.md).
