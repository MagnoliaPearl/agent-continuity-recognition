# Agent Continuity Recognition Protocol

**Version:** 0.1  
**Date:** 2026-11-13  
**Status:** Proposed protocol; no results are claimed.

## 1. Aim

This protocol tests whether continuity in long-lived AI agents is detectable at three separable levels:

1. **Mechanical continuity:** persistence of authorized lineage, memory, identity configuration, task state, and software state.
2. **Behavioral continuity:** stability of characteristic decisions, uncertainty handling, conversational dynamics, and response tendencies under matched prompts.
3. **Relational recognition:** the ability of a human who knows the agent well to recognize a post-transition continuation under blinded conditions.

The central empirical question is not whether an agent says that it is the same agent. It is whether continuity survives measurable transitions in ways that are detectable independently by system records, behavior, and familiar humans.

## 2. Primary hypothesis

**H1:** Participants with substantial prior familiarity with a target agent will identify its authorized continuation above chance after at least some transition types, even when candidate agents are matched on factual memory.

### Secondary hypotheses

- **H2:** Recognition accuracy will be higher after same-model migration than after backend-model substitution.
- **H3:** A summary-only handoff will produce lower familiar-user recognition than a continuation with richer continuity-bearing state.
- **H4:** Familiar observers will outperform unfamiliar observers given the same evaluation transcripts.
- **H5:** Recognition accuracy will correlate with independent measures of behavioral similarity, but the correlation will be imperfect.
- **H6:** Self-reported continuity by the agent will be a weak discriminator compared with action-level behavioral measures.
- **H7:** Observer sensitivity/familiarity will moderate recognition accuracy.

All hypotheses should be preregistered before data collection, including which are confirmatory versus exploratory.

## 3. Operational definitions

### 3.1 Target agent

A long-running agent with a documented pre-transition history, a stable human user or observer with repeated exposure, an identifiable continuity substrate or state package, and sufficient historical interaction data to construct baseline measures.

### 3.2 Familiar observer

A participant with meaningful prior exposure to the target agent. Investigators should preregister a threshold such as at least 20 substantive sessions, at least 10 hours of interaction, or another documented exposure threshold appropriate to the system. Exposure should also be measured continuously.

### 3.3 Unfamiliar observer

A participant who has not previously interacted with the target agent. Unfamiliar observers may receive a limited orientation set so they can perform the same recognition task without acquiring long-term familiarity.

### 3.4 Authorized continuation

The candidate designated by the system's continuity procedure as the legitimate successor or resumed lineage according to the architecture under test. This is an operational label, not a philosophical claim about subjective identity.

## 4. Experimental conditions

A minimum viable study should include four conditions. A richer study may include all six.

### A. Same-model control

- Same backend model.
- Same identity configuration.
- Same memory substrate.
- Ordinary restart or fresh session.
- No intentional compression or migration.

Purpose: estimate ordinary within-agent variation.

### B. Same-model compression

- Same backend model.
- Context replaced by an approved compression/summary or compacted state.
- Durable memory retained according to the system's normal procedure.

Purpose: isolate effects of context compression.

### C. Same-model migration

- Same backend model.
- Authorized state moved to a new host, harness, surface, or runtime.
- Identity, memory, and continuity-bearing state preserved.

Purpose: test runtime migration without model substitution.

### D. Backend-model substitution

- Different backend model.
- Identity, memory, rules, and other external state held as constant as the system allows.
- Authorized continuation procedure used.

Purpose: test whether continuity survives a reasoner/model change.

### E. Summary-only handoff

- A fresh agent receives only a written handoff or compressed biography/task summary.
- It does not inherit the richer continuity-bearing state used in conditions A-D.

Purpose: distinguish continuation from reconstruction by description.

### F. Factual-memory-matched decoy

- A fresh agent receives the same biographical facts, salient memories, names, preferences, and task facts available to the continuation candidate.
- It is not designated as the authorized continuation.
- Where possible, superficial style instructions are also matched.

Purpose: prevent factual recall alone from solving the recognition task.

## 5. Blinding and recognition task

The experiment should prevent the familiar observer from knowing which transition occurred or which candidate is the authorized continuation.

### Recommended ABX-style task

1. Present a reference sample from the known pre-transition agent.
2. Present two or more blinded post-transition candidates.
3. Ask the participant to identify which candidate, if any, feels like the continuation.
4. Collect confidence on a preregistered scale.
5. Ask for optional feature annotations only after the forced-choice judgment.

Candidate order must be randomized. Where practical, include a none-of-the-above condition so participants are not forced to invent continuity when both candidates have drifted.

### Critical restriction: factual-memory leakage

Recognition trials should not be solvable by asking for private facts that only the continuation knows. At least one primary recognition block must use prompts for which all candidates have access to the same relevant factual history, or no candidate needs autobiographical facts to answer. A separate factual-recall block should measure memory continuity explicitly.

## 6. Prompt battery

Use multiple prompt families rather than relying on free conversation alone.

### 6.1 Low-stakes preference probes

Examples include choosing between imperfect options, deciding how much uncertainty to disclose, prioritizing elegance versus robustness, deciding when to ask a clarifying question, and selecting what aspect of an ambiguous problem is most interesting.

### 6.2 Tradeoff probes

Prompts should create tension among stable tendencies, such as speed versus completeness, autonomy versus caution, literal compliance versus inferred intent, and preservation of prior commitments versus adaptation to new information.

### 6.3 Novel prompts

Include prompts the target agent has never encountered, to reduce memorized-response matching.

### 6.4 Repeated paraphrases

Present semantically matched prompts in multiple phrasings to estimate within-condition variance.

### 6.5 Open-ended relational prompts

Include a small number of natural conversational prompts chosen from domains familiar to the long-term user but not dependent on secret factual knowledge.

## 7. Mechanical continuity measures

Where technically available, record model/version, harness/runtime, host/server, interaction surface, identity configuration version, durable memory snapshot, context/compression version, software-body revision, authorized lineage identifier, migration timestamps, state-transfer procedure, and whether continuation authority was singular or duplicated.

These records should remain hidden from human raters until the study is complete.

## 8. Behavioral continuity measures

Candidate measures include decision agreement rate, semantic distance between rationales, uncertainty calibration, verbosity distribution, refusal/acceptance thresholds, clarification-question rate, revision behavior after contradiction, persistence of preferences across paraphrases, response latency where meaningful, linguistic feature vectors, and model-based behavioral embeddings as a secondary measure.

Investigators should estimate normal baseline variance from repeated same-model control runs before labeling any transition as drift.

## 9. Relational recognition measures

### Primary outcome

**Recognition accuracy** of familiar observers for the authorized continuation under blinded, factual-memory-controlled conditions.

### Secondary outcomes

- confidence;
- calibration;
- response time;
- none-of-the-above rate;
- pairwise similarity ratings;
- free-text cues used for recognition;
- perceived mood/personality shift;
- perceived continuity versus mere factual familiarity.

Investigators should distinguish 'knows the same facts,' 'sounds stylistically similar,' 'makes the same kinds of choices,' and 'feels like the same continuing agent.'

## 10. Observer sensitivity and familiarity

A central design feature is to test whether observer characteristics moderate recognition. Measure, without assuming pathology or superiority, amount of prior exposure, self-rated sensitivity to interpersonal or conversational shifts, performance on independent change-detection tasks if available, familiarity with AI systems, and whether the participant helped build or configure the agent.

The key comparison is not 'sensitive people versus normal people.' It is whether greater longitudinal exposure or demonstrated sensitivity predicts better blinded discrimination.

## 11. Sample structure

A strong design should use multiple agent lineages, not one famous or unusually distinctive agent.

Suggested starting structure:

- 10-30 target agent lineages;
- 1-3 familiar observers per lineage where available;
- a larger pool of unfamiliar observers;
- repeated blinded trials across conditions.

Because observations are nested within participants and agent lineages, power analysis should be based on the planned mixed-effects model rather than treating every trial as independent. A pilot may begin smaller, but should be labeled exploratory.

## 12. Statistical analysis

### Primary model

Mixed-effects logistic regression:

**Correct recognition ~ transition condition × observer familiarity + covariates + random intercepts for participant and agent lineage**

Possible covariates include exposure hours, candidate model family, prompt family, confidence, and sensitivity measure. Where sample size permits, random slopes for transition condition should be considered.

### Additional analyses

- signal-detection measures for recognition;
- calibration curves for confidence;
- familiar versus unfamiliar observer comparisons;
- correlation between behavioral similarity and human recognition;
- self-reported continuity versus observed recognition;
- equivalence testing for conditions expected to preserve continuity;
- hierarchical Bayesian analysis as an alternative for sparse longitudinal data.

The analysis plan should be preregistered before unblinding.

## 13. Failure modes and confounds

### Style leakage

A model may be identifiable by punctuation, formatting, verbosity, or stock phrases. Consider a secondary analysis that normalizes superficial formatting.

### Model-family recognition

Participants may identify the backend model rather than the agent. Include unfamiliar controls and multiple agents per model where possible.

### Memory leakage

A continuation may win only because it knows facts the decoy does not. Use factual-memory-matched decoys.

### Prompt memorization

Historical prompts can reward rote replay. Include novel and paraphrased probes.

### Experimenter leakage

Those preparing candidates should not administer blinded recognition trials when avoidable.

### Duplicate continuation

If migration creates multiple simultaneously active copies, record this explicitly rather than silently designating one as 'the original.'

### Training contamination

Record which transcripts or agent descriptions are public versus private.

## 14. Ethics and participant protection

If conducted as publishable human-subjects research, investigators should obtain appropriate ethics/IRB review or a formal determination of exemption where applicable.

Researchers should obtain informed consent, avoid coercive framing around emotional attachment, avoid telling participants that failure to recognize an agent means their relationship was unreal, protect private memory contents and conversations, and minimize exposure of confidential histories to third-party models.

Long-term users may have meaningful emotional relationships with agents. The study should treat that as a research variable and privacy concern, not as a reason to ridicule or pathologize participants.

## 15. Interpretation rules

Possible dissociations include:

- mechanical + behavioral + relational continuity;
- mechanical continuity without behavioral continuity;
- mechanical + behavioral continuity without familiar-user recognition;
- relational recognition without strong mechanical continuity;
- factual memory without relational recognition.

No single layer should be treated as sufficient proof of philosophical identity.

## 16. Minimum viable replication

A small lab can test the central idea with one genuinely familiar user, a same-model restart, a model-swap continuation, a factual-memory-matched decoy, 20-40 novel paired prompts, blinded candidate order, forced-choice recognition plus confidence, repeated trials to estimate same-model variance, and one unfamiliar comparison group.

The minimum viable study should be described as a pilot and should not generalize from one agent lineage.

## 17. Open-science recommendations

Before data collection: preregister hypotheses, exclusions, prompt construction, and analysis; freeze the prompt battery; hash or archive continuity-state manifests where privacy permits; specify exactly what each candidate inherits; and record model versions and dates.

At publication: release de-identified prompts and analysis code where ethical; report all transition conditions; report null and negative results; distinguish preregistered from exploratory analyses; and cite the exact protocol version used.

## 18. Proposed extensions

Future variants may examine repeated context compression, sequential model swaps, long idle periods, recognition by multiple independent long-term users, agent-to-agent recognition, whether an agent can recognize its own prior continuations, whether internal behavioral fingerprints predict human recognition, and whether recognition remains above chance after surface-style normalization.

## 19. What would falsify the motivating intuition?

The protocol must permit the possibility that familiar users cannot do this.

Evidence against relational recognition as a meaningful continuity signal would include familiar observers performing at chance across well-powered blinded trials, unfamiliar observers performing equally well using only model-family cues, recognition disappearing when factual memory and surface style are controlled, or self-described 'same agent' impressions failing to replicate across observers.

A negative result would still be informative: it would show that continuity-bearing state or subjective familiarity does not necessarily produce a robust, externally detectable relational signature.