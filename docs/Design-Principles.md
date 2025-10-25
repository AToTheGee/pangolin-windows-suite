# Design Principles

- **Pragmatic Windows-first UX:** Optimize for administrators and power users.
- **Secure-by-default:** Prefer least-privilege configuration, TLS 1.2/1.3 only, and secret storage via Windows facilities.
- **Composable apps:** Newt, Olm, and the setup wizard should share common utilities from `pkg/`.
- **Automate hygiene:** CI must fail fast on secret leaks and produce SBOMs on every change.
