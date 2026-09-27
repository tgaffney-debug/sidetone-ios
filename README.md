# Sidetone development build

Native iPhone radio panel and hold-to-talk control for vPilot on Windows. This is a development candidate, not yet accepted on physical devices.

This branch is a **cloud-build launcher**. The reviewed Sidetone implementation is stored in `sidetone-candidate.bundle`, a standard Git bundle containing source commit `c7b628b2b0be18ca8a628b6036ccb0bc65840369` and its delta from upstream `b40b22503113b71b5a2fc21a5fbe68ff728c5c14`. The surrounding source tree is the upstream baseline, not the Sidetone application.

The manual **Sidetone** workflow verifies the bundle and checks out that exact candidate before compiling or testing. It has read-only repository permission and does not publish a release. Build manifests identify the candidate source commit, which differs from the workflow launcher commit.

To inspect the candidate locally, fetch the bundle into this clone and check out FETCH_HEAD. The candidate includes setup instructions, protocol documentation, safety tests and build scripts.

Bundle SHA-256: `16fe7cf8f121fb40c1181f735f8678c7ad8de3f24d96c7bee0c995dc11edb8a0`

GitHub browser is signed in as tgaffney-debug; the connector is linked to another account. This source-bundle launcher enables platform builds without creating credentials or changing account access.

Microphone and headset remain on the Windows PC. iPhone installation still needs Apple signing. No installer or IPA should be treated as flight-ready until device acceptance.
