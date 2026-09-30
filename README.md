# Sidetone 0.3 improvement candidate

Native iPhone radio panel and hold-to-talk for vPilot on your Windows Ally.

This branch is a cloud-build launcher. The application source is stored in the standard Git bundle `sidetone-candidate.bundle`, source commit `9915f47cf1f85348a7663c525394ae85b61fc264`. The surrounding tree is the upstream baseline. The manual Sidetone workflow verifies the bundle and checks out the exact source declared in `sidetone-source.txt` before compiling, testing and archiving.

Bundle SHA-256: `c7949dff3e27f8d6258bb627ca4220307f1f8c3a98d21398e020cacf69ec7fc2`.

Improvements include radios visible at launch, a compact physical-hold PTT dock, one shared guided connection flow, favorite naming and recall, persistent frequency-entry actions, a reviewed status-only support summary, stricter pairing-response verification, PTT session replay handling and bounded main-socket sends. Native UI checks cover small and Pro iPhones plus the iPad dashboard.

Demo sends no live radio commands. Microphone/headset stay on the Ally. Device acceptance remains separate from native build/test success. Apple signing is required to install the unsigned IPA.
