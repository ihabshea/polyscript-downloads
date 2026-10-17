# Polyscript 0.2.0-beta.3 — Clearer contradictions and reliable indexing

This patch makes the contradiction inspector conservative and repairs local
semantic indexing for longer passages. It continues the experimental Apple
Silicon macOS 15+ preview channel.

## Contradiction inspector

- Candidates require explicit opposing positions about the same complete target,
  action, and stated scope. Shared words and unresolved references such as “it”
  or “this” no longer establish that two meetings discuss the same thing.
- Questions, assignments, hypothetical or qualified positions, idioms, compatible
  choices, and ordinary later decisions are excluded from candidate conflicts.
- Previously stored candidates are rechecked against authorized current source
  text when read. No re-indexing or source migration is needed for this correction.
- Every remaining pair explains the shared change and retains both complete
  source passages. This remains conservative English pattern matching and can
  miss implicit or paraphrased conflicts; an empty inspector does not prove agreement.

## Semantic search and graph reliability

- Indexing starts with fresh progress at zero and reports newly indexed passages,
  an already up-to-date index, or an empty authorized library explicitly.
- Saved embeddings are reused. Cancelling preserves completed batches so a later
  explicit build processes only missing vectors.
- Nomic's physical batch now matches its 2,048-token model context. Longer inputs
  within the existing first-4,000-character bound are tokenized locally, split into
  bounded pieces, and pooled into one vector per original passage. Keyword search
  continues to cover the full stored transcript.
- Local model HTTP failures identify the embedding or answer model and retain
  the HTTP status without exposing provider response bodies.
- Repeated conversational fragments use sparse topic-navigation links instead
  of a persistent quadratic clique. Current revision and authorization checks
  remain in force for every displayed relationship.

## Installation and limits

Quit Polyscript and replace the application bundle with this version. The local
library and models are stored separately. Back up the complete closed profile
before upgrading. This patch retains the existing schema-4 Polybase storage;
upgrading from older SQLite previews still follows the one-way migration described
in the installation guide. Original imported recordings and transcripts are not
modified by the upgrade or interview shutdown.

Release attachments record the exact source revision, checksum, package checks,
and synthetic qualification results. Synthetic multilingual embedding checks
establish bounded inference behavior, not multilingual retrieval quality.

This is an experimental ad-hoc-signed preview, not a notarized or fully qualified
general release. Physical installation, microphone permission, and manual
accessibility qualification remain separate. Hosted CI status is recorded in
the release receipt; local results must not be described as a hosted CI pass.
Fresh consent and agreed use remain mandatory. Detected interviews still
terminate the application and its workers immediately.

## Local qualification

All 169 core checks and all 32 bundled desktop scenarios passed with no skips, including the seven opt-in native scenarios. The 380-case fictional intelligence evaluation, correction/restart/withdrawal demonstration, packaged native inference and generated-speech checks passed on clean source `8441cdbeae5caecf51262d2b4706a20152f3d28f`. The ZIP passed CRC, contained path and symlink checks, exact application inventory/hash comparison and extracted strict deep signatures.

GitHub Actions did not start because of account billing/spending limits: https://github.com/ihabshea/polyscript/actions/runs/39044984933. This is not a hosted CI pass. Controlled physical qualification and the full beta milestone remain pending. The initial native desktop attempt exceeded its two-minute UI wait during cold Metal shader compilation; the complete rerun is reported above. First-use model initialization can take several minutes.

SHA-256: `681c4149a4babf938446051cdfe2a5404b78447b8bc251b4e068c33a0528bbbb`
