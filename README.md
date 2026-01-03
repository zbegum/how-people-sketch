# How People Really Sketch

Sketches from an exploratory study designed to challenge assumptions baked into mainstream sketch datasets. The collection focuses on **natural, in-context sketching**: context-dependent abstraction, incomplete marks, and adaptation to an audience during conversation.

## About

This repository contains sketch data from an exploratory study accompanying the paper:

> **A Critical Review of Sketch Collection Methods: Remembering How Humans Really Sketch**  

Many widely used sketch datasets (e.g., TU Berlin, QuickDraw) capture *decontextualized* drawings and often omit or ignore factors that shape sketching in real communication such as multimodality and audience. The paper discusses factors that shape sketching behavior and critically evaluates popular datasets in sketch recognition community and outlines practices for more naturalistic sketch collection. This dataset implements several of those practices. Note that this repository provides illustrative samples from an exploratory study to highlight how natural sketching can differ substantially from existing datasets; it is not intended as a training corpus.

## Data collection

**56 participants** (computer engineering students, ages 19–24) sketched on a **Wacom Cintiq 22HD** while conversing with an experimenter.

### Experimental conditions

| Condition | Description | Sketches |
|---:|---|---:|
| 1 | Storytelling, no visual contact (barrier) | 123 |
| 2 | Storytelling, with visual contact | 49 |
| 3 | Design task (planning + presentation) | 40 |

### Sketch types

| Sketch type | Count | Description |
|---|---:|---|
| `memory` | 94 | Personal memory or past experience |
| `fictional` | 59 | Imagined or invented scenario |
| `design` | 33 | Design ideation (Condition 3) |
| `information` | 21 | Explaining factual or procedural information |
| `problem_solving` | 5 | Solving a concrete design problem (Condition 3) |

## Procedure

Participants were asked to tell stories involving **memories**, **information**, or **fictional scenarios**. For the first 10 minutes, sketching was **not explicitly requested**; it typically emerged when participants felt it helped communication. If a participant did not sketch, they were later encouraged to "visualize the scene to help me understand." When participants struggled to choose a topic, we suggested **themes** (e.g., sailing, diving, car mechanic, baker, fitness) rather than specific objects. Participants then selected a memory, explanation, or fictional scenario related to the theme.

**Condition 1 (barrier).** A wooden barrier separated participant and experimenter—both could see the tablet but not each other directly.

**Condition 2 (no barrier).** The experimenter sat beside the participant, allowing eye contact and shared gaze.

**Condition 3 (design).** Participants identified a problem related to their hobbies and designed a solution. Some first sketched alone (planning phase) then explained their design on a new canvas (presentation phase); others did planning and presentation together.

## Observations

- **Drawing anxiety.** Some participants abandoned stick figures mid-drawing, restarted on a new canvas, or reported they "struggled with drawing" unless sketching was made mandatory.
- **Topic familiarity.** Familiar topics often elicited more confident sketching. Some participants could not proceed without a theme suggestion, or rejected multiple suggestions before selecting one they could work with.
- **Difficulty sketching while talking.** Several participants paused speech to draw silently; others struggled to do both simultaneously.
- **Self-initiated sketching.** When sketching emerged naturally, participants often framed it as "comfortable when explaining something I know," and gravitated toward content where visuals helped.
- **Audience adaptation.** Participants adjusted abstraction based on perceived experimenter knowledge—simplifying when a topic seemed shared, adding detail when it did not.

## Metadata

| Column | Description |
|---|---|
| `filename` | Sketch file name |
| `participant_id` | Anonymized ID (`P1`–`P56`) |
| `condition` | Experimental condition (`1`, `2`, or `3`) |
| `sketch_type` | `memory`, `fictional`, `design`, `information`, `problem_solving` |
| `self_initiated` | Whether sketching emerged without prompting |
| `content_summary` | Brief description of content and context  |

