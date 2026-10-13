# Polyscript 0.1.0-beta.4 — Live workspace and duplicate prevention

For Apple Silicon Macs running macOS 15 or later. Ad-hoc signed and not notarized.

- A dedicated live workspace with the full timestamped transcript, elapsed time, input level, processing and queue state, follow controls, and visible Finish/Withdraw actions.
- Exact and conservative almost-identical copy prevention within the same meeting date and timezone, including renamed recordings and bulk queues. Skipped results identify the original; repeated speech stays intact.
- Explicit transcript name prefixes and VTT voice tags become speaker labels. Older unlabeled prefixes are repaired while preserving timing and bookmarks and refreshing search. Speaker identities are never inferred from audio.
- Local recording fingerprints are removed when an original is edited, revoked or deleted. Unsaved duplicate state is limited to the current batch.
- Withdrawal during preparation or final processing suppresses late capture and output. Original files and existing meetings are never merged or overwritten by duplicate matching.

Bulk import, local speech, searchable meeting memory, source-linked questions, corrections, bookmarks and permitted export remain available. Duplicate matching and interview detection are heuristic and can misclassify; review source transcripts and skipped results.

Ask everyone involved for permission and agree on transcript use before every recording or import. Every repeated import still requires fresh confirmations. Do not use or share transcripts outside that agreement. Interview use is prohibited, even with consent; detection stops work and exits the app immediately.

The ZIP includes native runtimes, source archives, license notices and Electron/Chromium notices. It contains no model weights, recordings, saved meetings or development checkout. Model setup is explicit and processing stays local.

[Download](https://script.polymathlabs.xyz/download.html), [installation](https://script.polymathlabs.xyz/installation.html), [user guide](https://script.polymathlabs.xyz/docs.html), and [release history](https://script.polymathlabs.xyz/release-notes.html).

Verify the ZIP with the attached SHA256SUMS.txt. The ZIP is 196,586,598 bytes.

SHA-256: c95e639e003ce8fd3d774320770b1e46bec05d1fe6455b3ae6c4c0d1e9946760.
