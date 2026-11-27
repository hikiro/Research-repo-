# Animation, Context, Rigging, and QA Rulebook

This is an evidence-aware framework for organizing and testing rules. It is not a claim that every item below is a universal animation law. Promote a proposed rule to a stronger status only after gathering credible references or repeatable production evidence.

## 1. Action and intention

For each action, record:
- what the character wants or intends;
- what the character does;
- what changes as a result;
- which visual cues make the action readable;
- what the character or environment does in response.

Evaluate whether preparation, execution, contact, follow-through, and reaction are appropriate to the action. Not every action requires every phase or an exaggerated version of it.

## 2. Physical and spatial context

Record:
- character anatomy and body plan;
- mass distribution and balance assumptions;
- support surface and gravity direction;
- object dimensions, mass assumptions, attachment points, and affordances;
- contact points, constraints, resistance, and collision geometry;
- environment dimensions and obstacles;
- camera framing, perspective, screen direction, and visibility.

Do not diagnose a physical-looking animation from screen-space appearance alone when the underlying transforms or geometry can be inspected.

## 3. Rigging adaptation

A rig or motion preset must be adapted to the character rather than selected only by a broad label such as "biped" or "quadruped".

Document at least:
- morphology, proportions, and segment lengths;
- joint locations, axes, degrees of freedom, and limits;
- mass distribution and center-of-mass assumptions;
- support strategy and locomotion pattern;
- contact surfaces and expected object interactions;
- deformation requirements and anatomy-specific controls;
- character scale relative to props and environment;
- shot requirements and camera visibility;
- known failure modes and validation tests.

For a new creature or size, explicitly identify which parts of an existing rig or motion rule transfer, which need retuning, and which are not applicable. Do not assume that uniform scaling alone preserves believable mechanics.

## 4. Motion and visual readability

For each test, evaluate the motion in its intended context:
- silhouette and pose readability;
- intention and action clarity;
- timing and spacing;
- continuity and screen direction;
- balance and support;
- contact, attachment, and release;
- object response and follow-through;
- secondary motion where justified;
- framing and occlusion;
- sound and visual synchronization where applicable.

These are evaluation dimensions, not fixed prescriptions for every shot. Record the actual failure and evidence rather than assigning generic scores without criteria.

## 5. Scenario presets

Every scenario preset must specify:
1. scenario name and intended use;
2. character morphology and scale;
3. action and intention;
4. environment and object context;
5. rig and control assumptions;
6. motion and contact rules;
7. camera and framing;
8. audio requirements where relevant;
9. grounded references and evidence labels;
10. failure patterns and known limitations;
11. reproducible validation procedure;
12. version and change history.

Use [the scenario preset template](templates/SCENARIO_PRESET_TEMPLATE.md).

## 6. Evidence and promotion of rules

A rule entry must include:
- a precise, testable statement;
- the context and scope where it applies;
- source references or reproducible project tests;
- counterexamples, exceptions, and limitations;
- a validation method;
- date and revision history.

Keep hypotheses separate from validated rules. If new evidence contradicts a rule, preserve the old record and document the revision.

## 7. Production QA

Use both technical and visual checks where appropriate:
- source and asset provenance;
- deterministic build or test conditions;
- transform and geometry checks;
- contact/collision checks;
- frame-by-frame visual review;
- camera/framing review;
- render integrity and missing-frame checks;
- comparison against references;
- recorded pass/fail criteria.

A technical pass does not automatically establish artistic success; a visually pleasing frame does not automatically establish correct rig or contact behaviour.
