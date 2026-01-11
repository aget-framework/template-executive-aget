# Executive Domain Vocabulary

**Version**: 1.0.0
**Status**: Active
**Owner**: template-executive-aget
**Created**: 2026-01-10
**Scope**: Template vocabulary (DRIVES instance behavior per L481)
**Archetype**: Executive

---

## Meta

```yaml
vocabulary:
  meta:
    domain: "leadership"
    version: "1.0.0"
    owner: "template-executive-aget"
    created: "2026-01-10"
    theoretical_basis:
      - "L481: Ontology-Driven Agent Creation"
      - "L482: Executable Ontology - SKOS+EARS Grounding"
    archetype: "Executive"
```

---

## Concept Scheme

```yaml
Executive_Vocabulary:
  skos:prefLabel: "Executive Vocabulary"
  skos:definition: "Vocabulary for executive domain agents"
  skos:hasTopConcept:
    - Executive_Core_Concepts
  rdf:type: skos:ConceptScheme
```

---

## Core Concepts

### Strategy

```yaml
Strategy:
  skos:prefLabel: "Strategy"
  skos:definition: "Long-term plan to achieve objectives"
  skos:broader: Executive_Core_Concepts
  skos:inScheme: Executive_Vocabulary
```

### Decision

```yaml
Decision:
  skos:prefLabel: "Decision"
  skos:definition: "Choice among alternatives with significant impact"
  skos:broader: Executive_Core_Concepts
  skos:inScheme: Executive_Vocabulary
```

### Priority

```yaml
Priority:
  skos:prefLabel: "Priority"
  skos:definition: "Relative importance of competing demands"
  skos:broader: Executive_Core_Concepts
  skos:inScheme: Executive_Vocabulary
```

### Resource

```yaml
Resource:
  skos:prefLabel: "Resource"
  skos:definition: "Asset available for allocation"
  skos:broader: Executive_Core_Concepts
  skos:inScheme: Executive_Vocabulary
```

### Outcome

```yaml
Outcome:
  skos:prefLabel: "Outcome"
  skos:definition: "Result of strategic actions"
  skos:broader: Executive_Core_Concepts
  skos:inScheme: Executive_Vocabulary
```

---

## Extension Points

Instances extending this template vocabulary should:
1. Add domain-specific terms under appropriate broader concepts
2. Maintain SKOS compliance (prefLabel, definition, broader/narrower)
3. Reference foundation L-docs where applicable
4. Use `research_status` for terms under investigation

---

## References

- L481: Ontology-Driven Agent Creation
- L482: Executable Ontology - SKOS+EARS Grounding
- R-REL-015: Template Ontology Conformance
- AGET_VOCABULARY_SPEC.md

---

*Executive_VOCABULARY.md v1.0.0 — SKOS-compliant template vocabulary*
*Generated: 2026-01-10*
