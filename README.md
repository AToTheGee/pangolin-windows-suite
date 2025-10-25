# Pangolin Windows Suite

![Quality checks](https://github.com/AToTheGee/pangolin-windows-suite/actions/workflows/quality.yml/badge.svg)

## Was ist das?
Ein pragmatisches Windows-Toolkit für die Pangolin Newt- und Olm-Anwendungen plus Setup-Wizard. Aktuell stellen wir das Repo-Grundgerüst bereit: Ordnerstruktur, CI/Security-Hygiene und Release-Vorbereitung – noch keine App-Binaries.

## 90-Sekunden-Quickstart
1. **Klonen:** `git clone https://github.com/AToTheGee/pangolin-windows-suite.git` und in `feat/<topic>`-Branch arbeiten.
2. **Workflows prüfen:** Actions-Tab öffnen – `quality` erzeugt SBOM & Secret-Scan, `build` hält Platz für künftige Artefakte.
3. **Lokale Vorbereitung:** TODO-Skripte unter `scripts/` lesen (`dev-setup.ps1`, `build.ps1`, `release.ps1`) und offene Punkte in Issues festhalten.

## Status & Hygiene
- Struktur: `apps/`, `pkg/`, `docs/`, `scripts/` – alle mit Readme/Stub-Dateien.
- Security: gitleaks-Scan, SBOM via Syft, TLS-Policy in `SECURITY.md`.
- Branch-Modell: `main` stabil, `dev` integration, Feature-Branches nach `feat/<kurz>`.

## Roadmap (Nächste Schritte)
1. GUI-Mockups für Newt/Olm erstellen und Feedback einsammeln.
2. Setup Wizard Service-Installer konzipieren (WinGet/MSIX Evaluierung).
3. Build/Release-Skripte mit echten Artefakten (ZIP → MSIX → winget) füllen.

## FAQ (Auszug)
- **Wann kommen Builds?** Sobald Buildskripte stehen – Ziel: erste ZIP-Artefakte.
- **Wie melde ich Sicherheitsprobleme?** Siehe `SECURITY.md` (Responsible Disclosure E-Mail folgt).
- **Kann ich schon beitragen?** Ja! Siehe `CONTRIBUTING.md` und fokussiere dich auf Doku/Tooling.

## Lizenz
GPL-3.0 – siehe `LICENSE`.
