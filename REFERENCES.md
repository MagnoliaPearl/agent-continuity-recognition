# References and Related Work

This is a focused starting bibliography for protocol v0.1, not a complete literature review.

## Persistent-agent architecture

**Zhao, Z., & Zhao, R. (2026).** *Runtime-Independent Persistent Agents: Preserving Identity, Memory, and Code Across Models, Harnesses, and Servers.* arXiv:2609.00546.  
https://arxiv.org/abs/2609.00546

Relevance: separates a continuity-bearing substrate—identity, durable memory, and versioned software body—from replaceable model/runtime/surface bindings. The work explicitly limits its evidence to mechanical continuity rather than behavioral invariance, leaving a downstream measurement question that this protocol addresses.

## Behavioral drift under model transition

**Kang, Y., Huang, P.-C., Ku, C.-T., Hsu, C., Lee, P.-J., & Cheng, I.-L. (2026).** *Towards Identity-Preserving LLM Agents under Model Transition.* arXiv:2611.10628.  
https://arxiv.org/abs/2611.10628

Relevance: tests model substitution while holding external state constant and finds that some model transitions produce behavioral drift despite verbal claims of continued policy adherence. This motivates action-level continuity testing rather than relying on self-report.

## Human detection of behavioral drift

**Karny, S., Baez, A., & Pataranutaporn, P. (2026).** *Multi-Turn Neural Transparency: Surfacing Neural Activations Improves User Calibration to LLM Behavioral Drift.* arXiv:2605.15455.  
https://arxiv.org/abs/2605.15455

Relevance: randomized human-subject work (N=246) showing that ordinary users can struggle to evaluate changing personality-trait expression and that additional transparency can improve calibration. This motivates directly testing whether longitudinal familiarity changes human sensitivity to drift.

## Persona drift and relationship discontinuity

**How AI service persona drift erodes consumer trust through relationship discontinuity.** *Journal of Retailing and Consumer Services*, Volume 94, January 2027, 104985.  
https://doi.org/10.1016/j.jretconser.2026.104985

Relevance: conceptualizes persona drift across encounters as psychologically meaningful because users perceive a break in an established interaction pattern. This provides an adjacent human-relational framing for the proposed recognition endpoint.

## Research gap targeted here

The works above address persistent state and lineage, behavioral drift after model replacement, human evaluation of behavioral changes, and perceived persona discontinuity.

Protocol v0.1 targets the intersection that appears comparatively under-tested:

> **Can a human with substantial longitudinal familiarity recognize an authorized continuation of a specific agent after a blinded transition, when factual memory and superficial style are controlled?**

Additional references should be added as the literature search expands.