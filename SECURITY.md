# Sicherheitsrichtlinie

## Responsible Disclosure
- Vorläufige Kontaktadresse: `security@example.com` (Platzhalter, wird aktualisiert).
- Nutze PGP oder einen vertrauenswürdigen Kanal, teile keine Exploits öffentlich bevor ein Fix bereitsteht.

## Unterstützte Versionen
- `main` Branch (Scaffold-Phase)
- Release-Tags ab `v0.0.1`

## Sicherheitsgrundsätze
- **TLS:** Nur TLS 1.2/1.3 für zukünftige Netzwerk-Kommunikation.
- **Secret Storage:** Verwende Windows Credential Manager oder DPAPI; keine Klartext-Secrets im Repo.
- **CI-Hygiene:** `quality`-Workflow führt gitleaks-Scan aus und erzeugt eine SBOM via Syft.
- **Dependencies:** SBOM prüfen bevor Releases veröffentlicht werden.

## Meldeprozess
1. Problem privat melden.
2. Wir bestätigen innerhalb von 5 Werktagen.
3. Fix planen, veröffentlichen und Reporter informieren.
