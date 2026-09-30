# Sidetone 0.2 improvement candidate

Native iPhone radio panel and hold-to-talk for vPilot on your Windows Ally.

This branch is a cloud-build launcher. The application source is stored in the standard Git bundle `sidetone-candidate.bundle`, source commit `a78661e81fe11888e222531735912bbafae6c1dd`. The surrounding tree is the upstream baseline. The manual Sidetone workflow verifies the bundle and checks out the exact source declared in `sidetone-source.txt` before compiling, testing and archiving.

Bundle SHA-256: `9b2c0c3e823afca35ebf548a01b2cf7ad91821f5085e9ae07bf628ba1f6153d7`.

Improvements include guided connection setup, endpoint validation, adaptive cockpit, frequency favorites/recent requests, deliberate squawk entry, stale-state guards, bounded reconnection and actual simulator UI smoke tests. Demo cannot send live commands. Microphone/headset stay on the Ally. Device acceptance remains separate from native build/test success. Apple signing is required to install the unsigned IPA.
