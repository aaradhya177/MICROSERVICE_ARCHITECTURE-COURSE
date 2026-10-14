# Validation report

Validation date: 2026-10-14 (Asia/Calcutta)

Executed checks:

- `node --check dist/content.js` â€” passed.
- `node --check dist/app.js` â€” passed.
- Curriculum integrity script â€” passed: 30 modules, 90 unique lessons, 3 projects, 12 primary reference groups.
- Local static server request â€” passed with HTTP 200.
- Headless Chrome runtime check â€” passed after correcting a global lexical-name collision between content and application scripts.
- Browser visual inspection â€” limited because no controllable browser surface was available in the environment.

Limitations: embedded Go examples are teaching references drawn from the standard patterns described in their lessons; a full multi-service capstone repository is specified, not deployed as live infrastructure. External documentation can change after the verification date.

