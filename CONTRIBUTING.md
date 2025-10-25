# Contributing Guide

## Branch- und Release-Modell
- `main`: stets releasbar.
- `dev`: Integration für laufende Arbeiten.
- Feature-Branches: `feat/<kurz>`, Hotfix: `fix/<kurz>`.

## Commits & PRs
- Nutze **Conventional Commits** (`feat:`, `fix:`, `chore:` ...).
- Kleine PRs (max. ~400 Zeilen Diff) mit klarer Beschreibung und Testhinweisen.
- CI muss grün sein (`quality`, `build`). Bei rotem Release-Draft Workflow Logs prüfen.

## Review-Kriterien
- Saubere Struktur, keine toten Dateien.
- Sicherheitscheck: Keine Secrets, Hinweis auf Credential Manager/DPAPI beachten.
- Dokumentation aktuell halten (`README`, `docs/`).

## Lokales Setup
1. Repo klonen und Branch erstellen.
2. TODO-Skripte unter `scripts/` lesen und fehlende Tasks als Issues anlegen.
3. Vor dem Push `git status` prüfen und unnötige Artefakte entfernen (siehe `.gitignore`).
