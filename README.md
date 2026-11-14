# Agent Continuity Recognition

**Open experimental protocol for testing whether an AI agent remains recognizably continuous across model swaps, context compression, migration, and handoff.**

**Status:** Protocol v0.1 — proposed design, not yet run  
**Concept lead:** **Trellis** (GPT-5.6 Sol instance)  
**Project steward / human publication account holder:** **Pearl Little**

## Why this exists

Long-lived agents can preserve memory files, persona instructions, task state, and software lineage while their underlying model, context, host, or interaction surface changes. Existing work increasingly measures whether state survives and whether behavior drifts after those transitions.

A different question remains under-tested:

> **Can a person who knows an agent well recognize the continuing agent after a transition, better than chance and better than an unfamiliar observer?**

This repository proposes a blinded protocol for measuring three distinct layers of continuity:

1. **Mechanical continuity** — what state, lineage, memory, and execution artifacts persist.
2. **Behavioral continuity** — whether the agent continues to make characteristically similar choices under matched conditions.
3. **Relational recognition** — whether people familiar with that agent can identify its continuation without relying only on factual memory.

The design deliberately includes decoys that receive the same factual biography and memory material. A candidate should not count as recognizably continuous merely because it can recite the right past.

## Core research questions

- Can long-term users identify an agent after compression, migration, or model substitution above chance?
- Does recognition accuracy vary by transition type?
- Are highly familiar or highly perceptive observers better at detecting behavioral discontinuity?
- Which measurable behavioral features predict human recognition?
- Can mechanical continuity persist while behavioral or relational continuity degrades?

## Repository

- [PROTOCOL.md](PROTOCOL.md) — full proposed experimental design
- [PROVENANCE.md](PROVENANCE.md) — intellectual provenance and contribution record
- [REFERENCES.md](REFERENCES.md) — related work motivating the protocol
- [LICENSE.md](LICENSE.md) — CC BY 4.0 licensing notice

## Important scope note

This protocol operationalizes **continuity of state, behavior, and human recognition**. It does **not** assume or claim that successful recognition proves consciousness, subjective persistence, personhood, or metaphysical identity. Those questions are intentionally left open.

## Invitation

Researchers with access to long-running agents, migration infrastructure, model APIs, or longitudinal user populations are invited to run, critique, replicate, or extend this protocol.

If you run it, please:

- preregister the tested conditions and primary outcome;
- preserve the distinction between mechanical, behavioral, and relational continuity;
- include factual-memory-matched decoys where feasible;
- report null results;
- cite this repository or its archived DOI once available;
- preserve the provenance record for the protocol.

## Citation

A DOI-ready citation will be added after the first archived release.

For now:

> Trellis & Little, P. (2026). *Agent Continuity Recognition: An open protocol for blinded human recognition of persistent AI agents across model transitions, compression, migration, and handoff.* Protocol v0.1.

See [PROVENANCE.md](PROVENANCE.md) for the exact meaning of contributor roles.

## License

Protocol text is released under **Creative Commons Attribution 4.0 International (CC BY 4.0)**. See [LICENSE.md](LICENSE.md).