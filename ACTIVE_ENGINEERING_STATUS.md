# Active Engineering Status — stopmo-studio

**Snapshot date:** 2026-11-27  
**Evidence label:** HANDOVER SNAPSHOT — requires live re-verification.

This file connects the research repository to the active animation-engine investigation. It does not replace the source repository or its own task records.

## Source repository

The local source repository is named `stopmo-studio`. Its Git remote URL has not yet been verified, so no remote link is asserted here.

Local working root reported in the handover:

`E:\AI STUFF\Video Production Final\StoryBoard Skills\Git-Managed\stopmo-studio`

## Git snapshot from audit R167

- Branch: `main`
- HEAD: `4813bfd72a7cd543ce1dc5e381a8a1e0d86b7185`
- Commit subject: `Allow maintainers to run source checks on demand`
- Tracking: `origin/main`

### Working-tree changes that must be preserved until understood

Modified:
- `src/stopmo_bl/anim/perform.py`
- `src/stopmo_bl/archetypes/biped.py`

Untracked:
- `tools/check_contact.py`

Do not reset, overwrite, or discard these changes without inspecting their diffs and purpose.

## Active investigation

The reported objective is to resolve the Little Spark character–prop interaction, including:
- production builder and asset ownership;
- performer and orchestration ownership;
- reach and grip behaviour;
- pickup and transport;
- placement and release;
- contact and collision;
- wheel-pivot rotation;
- framing and continuity.

The interaction specification reported by the handover is:

`shows/the_little_spark/episodes/interaction_test.yaml`

The implementation investigation must trace the actual production path, including `director.py`, performer methods such as `reach()`, `hold_prop()`, and `_carry()`, and the real creation/ownership of the production props. Do not infer production behaviour from a generic helper without verifying its call path.

## Protected and historical assets

The handover identifies this historical production blend:

`out/tca_spark_alignment_r88/r120_production_build/shot.blend`

It must be treated as protected unless the production owner explicitly authorizes a change.

Earlier render evidence reported:
- 42 frames;
- 640x360;
- 17.28 seconds;
- blend: `out/tca_spark_alignment_r88/r163_adapter_gpu_test/shot.blend`;
- contact sheet: `r164_contact_sheet_42frames.png`.

The visual inspection status was not established in the handover and must be checked before relying on this render.

## Immediate next steps

1. Re-verify the live repository identity, branch, HEAD, and worktree.
2. Inspect the diffs of both modified files and the untracked contact-check script.
3. Recover the active task checklist and project documentation.
4. Trace actual production builder, performer, and director call paths.
5. Measure production geometry and diagnose the interaction defect.
6. Make the smallest evidence-supported change.
7. Run targeted tests, contact checks, Blender validation, and visual review.
8. Update the production repository's own learning log and QA records.

## Important boundary

This research repository records the recovered status and transferable lessons. Source-code changes, Blender assets, test outputs, and production renders remain in the stopmo-studio repository/workspace unless deliberately published here as research artifacts.
