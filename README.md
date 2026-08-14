# Annotation Guidelines for Pediatric Amblyopia

Reference guidelines for clinical annotators marking entities, relationships, and attributes in pediatric amblyopia ophthalmology notes, for a gold standard corpus annotated in INCEpTION. This is version 5.

The whole thing is one self-contained HTML file. Open `index.html` in a browser and it works, with no build step, no dependencies, and no network requests.

## Why a website

The first versions of these guidelines were a Word document. That is the wrong format for the job. An annotator hits an ambiguous span in the middle of a note and needs one specific rule in a few seconds, and scrolling a long document to find it breaks concentration every time. A single searchable page with a persistent table of contents and a decision flow answers the question where it gets asked.

Keeping it to one file matters for the same reason. Annotators are clinical staff, not developers. Anything that needs a server or an install will not get used.

## What it covers

The annotation model has three layers, and the guidelines are organized around them:

| Layer | What the annotator does |
|---|---|
| Spans | Mark the minimal continuous text expressing a concept, one label per span |
| Attributes | Set assertion, experiencer, and temporality, but only when the text explicitly indicates a non-default value |
| Relationships | Link spans the text connects, such as laterality to diagnosis or adherence to treatment |

The governing rule is to annotate what is written, not what the clinician appears to have meant. Missing laterality, missing time, and missing diagnoses are not inferred from context or from structured fields elsewhere in the note.

Most annotator disagreement in early rounds came from eligibility rather than labeling, so the guidelines lead with a decision flow for what counts as annotatable text at all. Narrative sections written by the clinician are eligible: HPI and interval history, assessment, plan and MDM. Structured blocks are not, even when they render as text, which covers visual acuity tables, refraction grids, and slit lamp template rows. Review of systems checklists are never eligible, including negations such as "denies blurred vision".

The remaining sections cover attribute defaults and their override triggers, worked examples, a quick reference, and the full concept inventory with color codes.

## Scope

This repository contains the guidelines only. No clinical notes, no annotations, and no corpus data are included here.
