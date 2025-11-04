# Handoff Process Between Modes

## Handoff Document Structure

Jedes Handoff-Dokument muss folgende Struktur haben:
```markdown
# Handoff: [Source Mode] → [Target Mode]

## Date & Context
- Date: [YYYY-MM-DD]
- Project: [Project Name]
- Feature: [Feature Name]
- Source Mode: [Mode Name]
- Target Mode: [Mode Name]

## Completed Work Summary
[Kurze Zusammenfassung der abgeschlossenen Arbeit]

## Key Deliverables
- [Deliverable 1]
- [Deliverable 2]
- ...

## Important Decisions
[Wichtige Entscheidungen, die getroffen wurden]

## Context for Next Phase
[Kontext und Informationen, die der nächste Mode benötigt]

## Open Questions
[Offene Fragen oder ungelöste Punkte]

## References
- [Link zu relevanten Dokumenten]
- [Link zu Code/Commits]
- ...

## Quality Gate Status
[Status aller Quality Gate Kriterien]

## Next Steps
[Was der nächste Mode tun sollte]
```

## Handoff Workflow

1. **Vor dem Handoff:**
   - Aktuelle Phase abschließen
   - Quality Gates überprüfen
   - Handoff-Dokument erstellen
   - Benutzer-Review durchführen

2. **Während des Handoffs:**
   - Handoff-Dokument in docs/handoffs/ speichern
   - Git Commit mit Phase-Tag erstellen
   - Zusammenfassung für Parent Task bereitstellen

3. **Nach dem Handoff:**
   - Nächster Mode liest Handoff-Dokument
   - Nächster Mode bestätigt Verständnis
   - Arbeit in nächster Phase beginnt