# Sidetone 0.2 improvement candidate

Native iPhone radio panel and hold-to-talk for vPilot on your Windows Ally.

This branch is a cloud-build launcher. The application source is stored in the standard Git bundle `sidetone-candidate.bundle`, source commit `4b85951063d96a80348a0ae6255478006d4a7f9f`. The surrounding tree is the upstream baseline. The manual Sidetone workflow verifies the bundle and checks out the exact source declared in `sidetone-source.txt` before compiling, testing and archiving.

Bundle SHA-256: `4ed80a4f25dc2cddc363ade6ebcbcd428a7b8563d7df54c2431871ff342ce34e`.

Improvements include guided connection setup, endpoint validation, adaptive cockpit, frequency favorites/recent requests, deliberate squawk entry, stale-state guards, bounded reconnection and actual simulator UI smoke tests. Demo cannot send live commands. Microphone/headset stay on the Ally. Device acceptance remains separate from native build/test success. Apple signing is required to install the unsigned IPA.
