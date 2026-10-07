# Imaginesis curriculum crosswalk — maths skills x national curricula x grades

Mapping of the official mathematics curriculum documents of 10 school systems to one shared
taxonomy of 417 maths skills, grade by grade. Prepared by Imaginesis (https://imaginesis.com),
a maths worksheet generator, and used there to pick worksheet topics for each country and grade.

Snapshot: 2026-10-07. License: Creative Commons Attribution 4.0 (CC BY 4.0) — cite as
"Imaginesis curriculum crosswalk, 2026, https://imaginesis.com/en/curricula".

## Files

- `data/skills.csv` — taxonomy: `slug`, `level` (1 domain, 2 topic, 3 skill), `parent_slug`, `name_en`, `name_pl`
- `data/curricula.csv` — `code`, `country` (ISO 3166-1), `name`, `sources` (official documents, space-separated URLs)
- `data/placements.csv` — `skill_slug`, `curriculum_code`, `grade_min`, `grade_max`, `program_code`
  (the requirement's identifier in the source document, when the document has one)

## How to read grades

Grade 1 = the first year of formal schooling in that country (Poland klasa 1 at age 7, England
Year 1 at age 5, elsewhere at age 6; grade 0 = the year before). Grade ranges reflect the
document: curricula written in cycles or key stages assign a skill to several years at once.

## Scope and limits

The mapping covers the skills the Imaginesis generator supports; a missing placement means
"not mapped", not "not taught". Several countries have more than one document (old and new
curriculum, different school tracks) — each is a separate row in `data/curricula.csv`.
