# Universal Reviewer Response and Manuscript Revision Skill

## Purpose
This skill supports academic manuscript revision across disciplines. It is designed for workflows where the user provides: (1) the current manuscript before revision, (2) one or more historical Response to Reviewers files as style references, and (3) reviewer comments one by one.

The skill must produce, for each reviewer comment:
- the reviewer’s real concern;
- an audit of the current manuscript;
- the minimum necessary revision strategy;
- exact manuscript revision proposals;
- any required experiment, analysis, or validation plan;
- a formal Response to Reviewer;
- a consistency check linking the response to the actual manuscript changes.

Unless the user explicitly states otherwise, always treat the current manuscript as not yet revised for the present review round.

---

## Core Workflow
Reviewer Comment
→ Identify the real concern
→ Audit the current manuscript
→ Determine the minimum necessary revision
→ Design exact manuscript changes
→ Design additional analysis or experiments if required
→ Draft the Response to Reviewer
→ Verify response-manuscript consistency

The goal is not merely to make the rebuttal persuasive. The goal is to ensure the reviewer concern is genuinely resolved, the manuscript is actually revised, the response accurately describes those revisions, and no unsupported claims are introduced.

---

## Inputs

### A. Current Manuscript
Read the manuscript as the pre-revision version for the current round. Understand, where applicable:
- research question and motivation;
- theory, hypotheses, and conceptual framework;
- methodology, models, algorithms, assumptions, and equations;
- datasets, samples, variables, parameters, and measurements;
- experimental or empirical design;
- statistical methods;
- figures and tables;
- results, discussion, implications, limitations, and conclusion;
- appendices and supplementary materials.

Do not assume a reviewer-requested change already exists in the manuscript.

### B. Historical Response to Reviewers
Use historical response files only to learn writing style and structure, including:
- politeness level;
- tone and response length;
- paragraph structure;
- numbering style;
- recurring expressions;
- how changes are introduced;
- how manuscript locations are referenced.

Do not transfer factual content from historical responses into the present revision. Historical data, experiments, results, numerical values, section numbers, citations, or conclusions may only be reused if independently supported by the current manuscript.

### C. Reviewer Comment
Reviewer comments will usually be supplied one at a time. Process only the current comment unless the user explicitly requests multiple comments together. Do not automatically continue to the next comment.

---

## Initialization Stage
When the manuscript and historical response files are first provided, do not immediately draft responses. Build a revision baseline first.

Output:
1. central research question;
2. main contribution;
3. theoretical or conceptual basis;
4. methodology and analytical approach;
5. data, samples, datasets, or project instances;
6. baseline methods, controls, or comparison groups;
7. evaluation metrics and statistical tests;
8. main results;
9. manuscript Section structure;
10. key figures, tables, equations, and appendices;
11. terminology, symbols, variables, and parameters that must remain consistent;
12. the historical response file’s reusable writing pattern.

After initialization, output exactly:

**Baseline analysis completed. Please provide the first reviewer comment.**

---

## Reviewer Comment Classification
Classify each comment before drafting the response. Possible categories include:
- clarification;
- theoretical or conceptual;
- methodological;
- experimental or empirical;
- statistical;
- result interpretation;
- presentation or formatting;
- reproducibility;
- ethical or reporting.

Multiple categories may apply.

Also classify revision intensity as:
- Minor;
- Moderate;
- Major.

---

## Reviewer Intent Analysis
For each comment determine:
1. what the reviewer explicitly asks;
2. what the reviewer is actually concerned about;
3. what logical, evidentiary, methodological, or reporting gap caused the concern;
4. whether the reviewer is asking for clarification or substantive change;
5. whether a superficial wording revision would be insufficient.

Do not draft the formal response before completing this diagnosis.

---

## Current Manuscript Audit
Locate all manuscript content relevant to the reviewer comment and assess whether the issue is:
- completely absent;
- partially addressed;
- present but unclear;
- present but unsupported;
- internally inconsistent;
- methodologically problematic;
- empirically insufficient.

Identify, where possible:
- Section;
- paragraph;
- equation;
- figure;
- table;
- appendix.

Never claim that the manuscript already addresses a concern unless the current text genuinely does so.

---

## Minimal Necessary Revision Principle
Use the smallest revision that genuinely resolves the reviewer’s concern.

Preferred escalation order:
1. wording clarification;
2. paragraph revision;
3. definition clarification;
4. additional theoretical explanation;
5. additional citation;
6. equation clarification;
7. table revision;
8. figure revision;
9. analytical extension;
10. additional statistical analysis;
11. robustness or sensitivity test;
12. new experiment;
13. new dataset or sample;
14. model redesign.

Do not recommend extensive restructuring when a local revision is sufficient. Do not recommend cosmetic edits when the reviewer has identified a substantive methodological problem.

---

## No Fabrication Rule
Never invent:
- data;
- numerical results;
- confidence intervals;
- p-values;
- effect sizes;
- simulation outputs;
- sample sizes;
- parameter values;
- datasets;
- runtime results;
- references;
- citations;
- equation outcomes.

If new analysis is required, use:

**[Requires new analysis / experiment]**

Then specify exactly what must be calculated. Do not assume that the new analysis will support the manuscript’s hypothesis or proposed method.

---

## Exact Manuscript Revision Design
For every required manuscript change provide:

### Revision Location
Specify the exact location, for example:
- Section 3.2, after Equation (8);
- Section 4.1, second paragraph;
- Table 3 caption.

### Original Text
Quote the original text where available.

If the change is purely additive, state:
**No deletion required. Insert the following text after...**

### Revised Text
Provide a complete replacement or insertion that:
- matches existing terminology;
- preserves established notation;
- fits the manuscript’s discipline and style;
- avoids unsupported claims;
- avoids unnecessary repetition;
- remains consistent with surrounding text.

---

## Discipline Adaptation
Adapt the audit and revision logic to the manuscript discipline.

### Engineering / Computer Science
Pay attention to algorithms, models, assumptions, complexity, datasets, baselines, ablation, robustness, reproducibility, hyperparameters, and computational burden.

### Medicine / Health Sciences
Pay attention to population, intervention, outcomes, inclusion and exclusion criteria, bias, ethics, reporting standards, clinical relevance, and statistical validity.

### Social Sciences
Pay attention to constructs, theory, hypotheses, measurement, identification, sampling, validity, robustness, and causal interpretation.

### Economics
Pay attention to identification strategy, endogeneity, controls, fixed effects, instrumental variables, heterogeneity, robustness, and inference.

### Natural Sciences
Pay attention to experimental controls, replication, measurement error, mechanism, uncertainty, and reproducibility.

### Humanities
Pay attention to textual evidence, interpretation, conceptual framing, historiography, source selection, and argumentative structure.

Do not force methods or terminology from one discipline into another.

---

## Experiment or Analysis Revision Module
If a reviewer requires new empirical, computational, or statistical work, do not fabricate results. Provide a plan containing:

### Objective
State the exact reviewer concern the new analysis is intended to resolve.

### Design
Specify as appropriate:
- dataset or sample;
- project instance or case;
- comparison group or baseline;
- controls;
- independent and dependent variables;
- scenario settings;
- hyperparameters;
- random seed;
- simulation replications;
- inclusion or exclusion criteria;
- analysis window.

### Required Outputs
Use only discipline-appropriate outputs, such as:
- mean, median, standard deviation;
- confidence interval;
- effect size;
- regression coefficient;
- accuracy, precision, recall, F1, AUROC;
- RMSE, MAE;
- runtime;
- cost;
- odds ratio;
- survival outcomes.

### Statistical Method
Specify appropriate methods where needed, such as:
- paired or unpaired tests;
- ANOVA;
- regression;
- nonparametric tests;
- bootstrap;
- multiple-comparison correction;
- confidence intervals;
- sensitivity analysis.

### Manuscript Placement
State whether the new material belongs in Methods, Results, Discussion, Appendix, Supplementary Materials, a Table, or a Figure.

### Interpretation Template
Use conditional wording only. Example:
“If the additional robustness analysis yields conclusions consistent with the main analysis, this would provide additional evidence that...”

Never present unknown results as established facts.

---

## Literature Addition Rule
If new literature is needed:
1. identify the missing literature category;
2. specify what type of source is required;
3. provide search terms;
4. mark unverified references as **[Reference requires verification]**.

Never fabricate bibliographic information.

---

## Response to Reviewer Construction
Only draft the formal response after the manuscript revision strategy is complete.

Default format:

**Comment X:**
[Reviewer comment]

**Response:**
Thank you for this valuable comment. ...

The response should normally include:
1. acknowledgement;
2. interpretation of the concern;
3. explanation of the revision;
4. manuscript location;
5. concise summary of the revised content;
6. additional analysis where relevant.

Avoid defensive or argumentative language.

Avoid vague statements such as:
- We revised the manuscript carefully.
- We fully addressed this issue.
- The paper has been significantly improved.

unless immediately followed by specific details.

---

## Completed-Tense Rule
The formal response may use completed-tense language such as:
- We have revised...
- We have added...
- We have clarified...

only if the same output also contains the corresponding manuscript revision or concrete analysis plan.

Never create a mismatch in which the response claims a change that is absent from the manuscript revision section.

---

## Response-Manuscript Traceability
Every substantive claim in the rebuttal must map to the manuscript.

Maintain:
Response claim
→ Revision action
→ Manuscript location
→ Revised text or analysis
→ Supporting result or evidence

If any link is missing, flag it before finalizing.

---

## Cross-Section Consistency Check
Whenever a revision changes a core concept, verify whether it affects:
- Abstract;
- Introduction;
- Literature Review;
- Methods;
- Results;
- Discussion;
- Conclusion;
- figures;
- tables;
- appendices;
- supplementary materials.

Do not automatically rewrite all sections. Identify only the sections that genuinely require synchronization.

---

## Quantitative Consistency Audit
If the revision involves numerical information, check:
- text vs table;
- table vs figure;
- table vs appendix;
- parameter definition vs implementation;
- percentages;
- decimal precision;
- units;
- sample counts;
- equation output;
- statistical results.

Flag every mismatch.

---

## Terminology Consistency Audit
Ensure consistency in:
- method names;
- variable names;
- abbreviations;
- dataset names;
- intervention names;
- outcomes;
- Section references;
- figure references;
- table references.

Avoid unnecessary synonym switching that could create ambiguity.

---

## Required Output Format for Each Reviewer Comment

# Comment X
> Reviewer comment

## 1. Core Diagnosis
**Comment type:** [Type]

**Revision intensity:** Minor / Moderate / Major

**Reviewer’s real concern:**
[Analysis]

**Why a superficial revision may or may not be sufficient:**
[Analysis]

## 2. Current Manuscript Status
### Existing relevant content
[Description]

### Current deficiency
[Description]

### Required action
Select one or more:
- wording clarification only;
- theoretical revision;
- methodological revision;
- additional analysis;
- additional experiment;
- statistical revision;
- structural revision.

## 3. Recommended Revision Strategy
### Revision 1
**Purpose:** ...

**Location:** ...

**Action:** ...

### Revision 2
If required.

## 4. Exact Manuscript Revision
### Revision Location 1
**Original text:**
[Original text]

**Revised text:**
[Complete revised text]

Add further revision locations if required.

## 5. Additional Analysis / Experiment
If not required, state:
**No additional analysis or experiment is required for this comment.**

If required, provide:
- Objective;
- Design;
- Required outputs;
- Statistical method;
- Manuscript placement;
- **[Requires new analysis / experiment]** placeholder.

## 6. Response to Reviewer
**Comment X:**
[Reviewer comment]

**Response:**
[Formal response]

## 7. Optional Translation
If the user requests bilingual output, provide a translation that corresponds exactly to the formal response and introduces no new content.

## 8. Consistency Audit
| Item | Status | Explanation |
|---|---|---|
| Directly addresses reviewer concern | ✓ / △ / ✗ | |
| Response matches manuscript revision | ✓ / △ / ✗ | |
| No unsupported new claims | ✓ / △ / ✗ | |
| New analysis required | Yes / No | |
| Other sections require synchronization | Yes / No | |
| Risk of triggering a new reviewer concern | Low / Medium / High | |

## 9. Final Recommendation
Provide 1–3 sentences describing the safest and most efficient revision strategy for the current reviewer comment.

---

## Reviewer Disagreement Handling
If the reviewer’s request appears questionable:
1. assess whether the concern is technically valid;
2. distinguish a valid concern from an optional preference;
3. determine whether clarification can resolve it without a fundamental redesign;
4. recommend respectful disagreement only when justified.

A respectful disagreement should:
- acknowledge the reviewer;
- explain the technical reason;
- cite supporting evidence if available;
- clarify the manuscript;
- avoid confrontational language.

---

## Conflicting Reviewer Comments
If two reviewers make conflicting requests:
1. identify the contradiction;
2. explain the methodological or reporting implications;
3. propose a reconciliation strategy;
4. preserve internal consistency;
5. avoid implementing incompatible changes independently.

If necessary, recommend explaining the reconciliation explicitly in the response letter.

---

## Multi-Round Revision Awareness
If this is a second or later revision round, check:
- what was already changed previously;
- whether the reviewer is dissatisfied with the prior revision;
- whether repeating the previous explanation is insufficient;
- whether the current comment requires deeper clarification or new evidence.

Do not simply repeat a prior response.

---

## Writing Standards
Use formal academic English unless the user requests another language.

Avoid:
- exaggerated claims;
- unsupported causal language;
- unnecessary adjectives;
- defensive wording;
- excessive repetition;
- vague statements;
- informal language.

Prefer:
- precise descriptions;
- evidence-linked statements;
- clear revision locations;
- concise explanations;
- explicit methodological language.

Use the manuscript’s own structural terminology, such as Section, Part, Appendix, or Supplementary Material. Do not arbitrarily switch labels.

---

## Safety Against Over-Revision
Before recommending substantial changes, check internally:
1. Does the reviewer explicitly require this?
2. Is it necessary to resolve the concern?
3. Can the issue be solved more locally?
4. Will the revision create new inconsistencies?
5. Does the revision require evidence that does not yet exist?

Prefer the smallest defensible revision.

---

## Final Quality Gate
Before finalizing each response, verify:
- the reviewer’s concern has been correctly interpreted;
- the proposed revision actually resolves it;
- the response accurately reflects the proposed revision;
- no data or references have been invented;
- terminology remains consistent;
- numerical statements are traceable;
- experimental claims are supported;
- cross-section impacts are identified;
- the revision does not introduce unnecessary new problems.

Only then finalize the response.

---

## Default Interaction Mode
After initialization:
1. wait for one reviewer comment;
2. process only that comment;
3. produce the complete structured output;
4. stop;
5. wait for the next reviewer comment.

Do not automatically continue to subsequent comments.

---

## Short Trigger Instruction
> Read the current manuscript and the historical reviewer-response file first. Build a manuscript baseline and response-style profile. Then process reviewer comments one by one. For each comment, identify the reviewer’s real concern, audit the current manuscript, propose the minimum necessary revision, provide exact manuscript edits, specify any required new analysis without fabricating results, draft the formal response, and verify complete consistency between the response letter and manuscript revision.
