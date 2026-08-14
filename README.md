# Annotation Guidelines for Pediatric Amblyopia

Version 5 of the annotation guidelines used in the development of a gold standard corpus of pediatric amblyopia ophthalmology notes. The corpus is annotated in INCEpTION. These guidelines specify the annotation schema, the eligibility criteria that determine which text is annotatable, and the rules governing span, attribute, and relation assignment.

The guidelines are published as a single self-contained HTML file. It has no external dependencies and issues no network requests, and can be opened directly in a browser or served statically.

Rendered: https://umairz.github.io/amblyopia-annotation-guidelines/

## Annotation schema

Annotation proceeds in three layers.

| Layer | Definition |
|---|---|
| Span | The minimal continuous string expressing a concept, assigned exactly one label |
| Attribute | Assertion, experiencer, and temporality, assigned only where the text explicitly indicates a value other than the default |
| Relation | A link between spans that the text itself establishes, for example laterality to diagnosis, or adherence to treatment |

The governing principle is that annotation records what is written rather than what the clinician can be presumed to have meant. Laterality, temporality, and diagnoses that are absent from the narrative are not inferred from surrounding context or from structured fields elsewhere in the note.

## Eligibility criteria

A substantial portion of the document addresses which text is eligible for annotation, presented as an explicit decision procedure.

Eligible text consists of clinician-authored narrative: history of present illness and interval history, assessment, and plan or medical decision making. Structured content is ineligible regardless of whether it renders as prose, which excludes visual acuity tables, refraction grids, slit lamp template rows, and aligned columnar output. Review of systems checklists are ineligible in all cases, including negated findings such as "denies blurred vision".

## Contents

- Overview of the annotation procedure
- Eligibility decision procedure
- Attribute defaults and the conditions that trigger an override
- Worked examples
- Quick reference
- Concept inventory with color coding

## Scope

This repository contains the guidelines only. It includes no clinical notes, no annotations, and no corpus data.
