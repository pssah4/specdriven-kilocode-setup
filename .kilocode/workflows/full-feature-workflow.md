# Complete Feature Development Workflow

Dieser Workflow orchestriert die komplette Feature-Entwicklung durch alle Phasen.

## Workflow Steps

1. **Initialize Project Context**
   - Erstelle Feature-Branch
   - Initialisiere Dokumentationsstruktur
   - Erstelle Issue für Feature-Tracking

2. **Business Analysis Phase**
   - Wechsel zu Business Analyst Mode: `new_task(mode="business-analyst")`
   - Analysiere Geschäftsanforderungen
   - Erstelle Business Case
   - Dokumentiere Stakeholder-Erwartungen
   - Erstelle BA → RE Handoff
   - Commit: `git commit -m "feat(ba): complete business analysis"`

3. **Requirements Engineering Phase**
   - Wechsel zu Requirements Engineer Mode: `new_task(mode="requirements-engineer")`
   - Lese BA Handoff
   - Erstelle detaillierte Requirements
   - Definiere Akzeptanzkriterien
   - Erstelle RE → Arch Handoff
   - Commit: `git commit -m "feat(re): complete requirements specification"`

4. **Architecture Phase**
   - Wechsel zu Architect Mode: `new_task(mode="architect")`
   - Lese RE Handoff
   - Designe System-Architektur
   - Erstelle ADRs für wichtige Entscheidungen
   - Aktualisiere ARC42 Dokumentation
   - Erstelle Arch → Code Handoff
   - Commit: `git commit -m "feat(arch): complete architecture design"`

5. **Implementation Phase**
   - Wechsel zu Code Mode: `new_task(mode="code")`
   - Lese Architecture Handoff
   - Implementiere Features
   - Schreibe Tests
   - Dokumentiere Code
   - Erstelle Code → Debug Handoff
   - Commit: `git commit -m "feat(code): implement [feature-name]"`

6. **Debug & Quality Assurance Phase**
   - Wechsel zu Debug Mode: `new_task(mode="debug")`
   - Lese Code Handoff
   - Führe alle Tests aus
   - Debugge und fixe Probleme
   - Verifiziere Requirements
   - Erstelle Qualitätsbericht
   - Commit: `git commit -m "test: verify and fix all issues"`

7. **Final Review**
   - Sammle alle Deliverables
   - Erstelle Abschlussbericht
   - Tag Release: `git tag -a v1.0.0 -m "Feature complete"`
   - Update Issue Status

## Quality Gate Checkpoints

Nach jedem Schritt:
- Führe `/quality-gate-check.md` Workflow aus
- Hole Benutzer-Freigabe ein
- Erstelle Handoff-Dokument
- Commit Phase-Ergebnisse

## Tools Used

- `new_task()`: Erstelle Subtask in anderem Mode
- `read_file()`: Lese Handoff-Dokumente
- `write_file()`: Erstelle Deliverables
- `execute_command()`: Git-Befehle, Tests ausführen
- `ask_followup_question()`: Nutzer-Feedback einholen