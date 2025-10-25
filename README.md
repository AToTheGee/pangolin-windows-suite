# Pangolin Windows Suite

![Quality checks](https://github.com/AToTheGee/pangolin-windows-suite/actions/workflows/quality.yml/badge.svg)

## Was ist das?
Ein pragmatisches Windows-Toolkit für die Pangolin Newt- und Olm-Anwendungen plus Setup-Wizard. Aktuell stellen wir das Repo-Grundgerüst bereit: Ordnerstruktur, CI/Security-Hygiene und Release-Vorbereitung – noch keine App-Binaries.

## 90-Sekunden-Quickstart
1. **Klonen:** `git clone https://github.com/AToTheGee/pangolin-windows-suite.git` und in `feat/<topic>`-Branch arbeiten.
2. **Workflows prüfen:** Actions-Tab öffnen – `quality` erzeugt SBOM & Secret-Scan, `build` hält Platz für künftige Artefakte.
3. **Lokale Vorbereitung:** Skripte unter `scripts/` lesen (`dev-setup.ps1`, `build.ps1`, `release.ps1`) und offene Punkte in Issues festhalten.

## Strukturüberblick
- `apps/` – Modul-Readme plus Platzhalter für Newt GUI, Olm GUI und Setup Wizard.
- `pkg/` – Geplante Shared Utilities für Dienste, Logging & Konfiguration.
- `docs/` – Dokumentationsdrehkreuz mit Leitlinien, Roadmaps und Troubleshooting.
- `scripts/` – PowerShell-Automatisierung für Setup, Build und Release.

## Status & Hygiene
- Security: gitleaks-Scan, SBOM via Syft, TLS-Policy in `SECURITY.md`.
- Branch-Modell: `main` stabil, `dev` integration, Feature-Branches nach `feat/<kurz>`.
- Release-Vorbereitung: Draft Notes in `docs/Release-Notes-Draft.md`.

## Roadmap (Nächste Schritte)
1. GUI-Mockups für Newt/Olm erstellen und Feedback einsammeln.
2. Setup Wizard Service-Installer konzipieren (WinGet/MSIX Evaluierung).
3. Build/Release-Skripte mit echten Artefakten (ZIP → MSIX → winget) füllen.

## FAQ (Auszug)
- **Wann kommen Builds?** Sobald Buildskripte stehen – Ziel: erste ZIP-Artefakte.
- **Wie melde ich Sicherheitsprobleme?** Siehe `SECURITY.md` (Responsible Disclosure E-Mail folgt).
- **Kann ich schon beitragen?** Ja! Siehe `CONTRIBUTING.md` und fokussiere dich auf Doku/Tooling.

## English Overview
The Pangolin Windows Suite is a pragmatic toolkit that will bundle the Newt and Olm desktop applications together with a unified setup wizard. Right now the repository provides the skeleton: directory layout, CI/security hygiene, and release preparation—application binaries will follow later.

### Quickstart
1. **Clone:** `git clone https://github.com/AToTheGee/pangolin-windows-suite.git` and work on `feat/<topic>` branches.
2. **Check workflows:** The `quality` workflow generates SBOMs and secret scans; `build` stands ready for future artefacts.
3. **Prep locally:** Review the PowerShell scripts in `scripts/` (`dev-setup.ps1`, `build.ps1`, `release.ps1`) and capture open tasks as issues.

### Repository layout
- `apps/` – Module index with placeholders for the Newt GUI, Olm GUI, and Setup Wizard projects.
- `pkg/` – Shared utilities planned for Windows services, logging, and configuration.
- `docs/` – Centralised documentation hub with design notes, troubleshooting, and release planning.
- `scripts/` – Automation entry points for developer setup, builds, and releases.

### Current focus
- Security hygiene via gitleaks and Syft SBOM generation.
- Branching model with a stable `main`, integration on `dev`, and feature branches named `feat/<short>`.
- Drafting release notes in `docs/Release-Notes-Draft.md` while implementation evolves.

### Roadmap
1. Produce GUI mock-ups for Newt/Olm and gather feedback.
2. Design the Setup Wizard service installer (evaluate WinGet/MSIX).
3. Flesh out build/release scripts once real artefacts (ZIP → MSIX → winget) are available.

### FAQ
- **When will builds ship?** As soon as the build scripts solidify—first target is ZIP artefacts.
- **How do I report security issues?** See `SECURITY.md` (dedicated disclosure mailbox coming soon).
- **Can I contribute now?** Absolutely. Start with docs/tooling updates via `CONTRIBUTING.md`.

## Lizenz
GPL-3.0 – siehe `LICENSE`.
