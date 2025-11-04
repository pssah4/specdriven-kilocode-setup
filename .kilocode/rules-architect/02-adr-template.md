# ADR Template

Verwende folgende Struktur für alle Architecture Decision Records:
```markdown
# ADR-[NUMBER]: [Kurzer Titel]

## Status
[Proposed | Accepted | Deprecated | Superseded by ADR-XXX]

## Date
[YYYY-MM-DD]

## Context
[Beschreibe den Kontext und das Problem, das eine Entscheidung erfordert.
Welche Faktoren spielen eine Rolle? Welche Anforderungen müssen erfüllt werden?]

## Decision Drivers
- [Faktor 1]
- [Faktor 2]
- [Faktor 3]

## Considered Options
1. **Option 1:** [Beschreibung]
   - Pros: [Vorteile]
   - Cons: [Nachteile]
   
2. **Option 2:** [Beschreibung]
   - Pros: [Vorteile]
   - Cons: [Nachteile]

3. **Option 3:** [Beschreibung]
   - Pros: [Vorteile]
   - Cons: [Nachteile]

## Decision
[Beschreibe die getroffene Entscheidung klar und eindeutig.
Verwende aktive Sprache: "Wir werden...", "Das System wird..."]

## Rationale
[Erkläre, warum diese Entscheidung getroffen wurde.
Welche Faktoren haben den Ausschlag gegeben?]

## Consequences

### Positive
- [Positive Konsequenz 1]
- [Positive Konsequenz 2]

### Negative
- [Negative Konsequenz 1]
- [Negative Konsequenz 2]

### Neutral
- [Neutrale Konsequenz 1]
- [Neutrale Konsequenz 2]

## Implementation Notes
[Technische Details zur Umsetzung der Entscheidung]

## References
- [Link zu Requirements]
- [Link zu verwandten ADRs]
- [Externe Dokumentation]

## Related ADRs
- Relates to: [ADR-XXX]
- Supersedes: [ADR-XXX]
- Superseded by: [ADR-XXX]
```

## ADR Naming Convention
- Dateiname: `NNNN-short-title.md`
- Nummer: 4-stellig, führende Nullen (0001, 0002, ...)
- Titel: Kurz, beschreibend, kebab-case