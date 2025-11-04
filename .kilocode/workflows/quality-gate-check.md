# Quality Gate Check Workflow

Dieser Workflow überprüft alle Quality Gate Kriterien für die aktuelle Phase.

## Steps

1. **Identify Current Phase**
   - Bestimme aktive Phase aus Kontext
   - Lade entsprechende Quality Gate Kriterien

2. **Check All Criteria**
   - Lese `.kilocode/rules/quality-gates.md`
   - Überprüfe jedes Kriterium für die aktuelle Phase
   - Dokumentiere Status (✓ erfüllt / ✗ nicht erfüllt)

3. **Generate Report**
   - Erstelle Quality Gate Report
   - Liste erfüllte Kriterien
   - Liste nicht erfüllte Kriterien
   - Gebe Empfehlungen für Verbesserungen

4. **User Review**
   - Präsentiere Report dem Nutzer
   - Hole Feedback ein mit `ask_followup_question()`
   - Dokumentiere User-Entscheidung

5. **Decision**
   - Wenn alle Kriterien erfüllt: Freigabe für nächste Phase
   - Wenn Kriterien fehlen: Liste erforderliche Aktionen
   - Aktualisiere Handoff-Dokument mit QG-Status

## Output

Erstelle Datei: `docs/quality-gates/qg-[phase]-[date].md`
```markdown
# Quality Gate Report: [Phase Name]

## Date: [YYYY-MM-DD]
## Phase: [Phase Name]

## Criteria Status

### Fulfilled ✓
- [Kriterium 1]
- [Kriterium 2]

### Not Fulfilled ✗
- [Kriterium 3] - [Grund]
- [Kriterium 4] - [Grund]

## Recommendations
[Empfehlungen zur Erfüllung fehlender Kriterien]

## User Decision
[Approved / Needs Work / Deferred]

## Next Steps
[Was als nächstes zu tun ist]
```