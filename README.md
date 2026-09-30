# Sidetone 0.2 improvement candidate

Native iPhone radio panel and hold-to-talk for vPilot on your Windows Ally.

This branch is a cloud-build launcher. The application source is stored in the standard Git bundle `sidetone-candidate.bundle`, source commit `ddf54cc9e3fb53619ea1a5bf544bcb9e68ebf426`. The surrounding tree is the upstream baseline. The manual Sidetone workflow verifies the bundle and checks out the exact source declared in `sidetone-source.txt` before compiling, testing and archiving.

Bundle SHA-256: `a8a8e9465ba26893558d69d28bf4bb269113d37564789095281f93a8e0f3d640`.

Improvements include guided connection setup, endpoint validation, adaptive cockpit, frequency favorites/recent requests, deliberate squawk entry, stale-state guards, bounded reconnection and actual simulator UI smoke tests. Demo cannot send live commands. Microphone/headset stay on the Ally. Device acceptance remains separate from native build/test success. Apple signing is required to install the unsigned IPA.
