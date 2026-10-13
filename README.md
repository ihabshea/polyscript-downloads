# Polyscript Mac downloads

Polyscript turns permitted conversations into local transcription and searchable,
source-linked meeting memory. [Meet Polyscript](https://script.polymathlabs.xyz/).

This repository hosts executable downloads and distribution documentation.

## Experimental Mac preview

[Download Polyscript 0.1.0-beta.1 for Apple Silicon](https://github.com/ihabshea/polyscript-downloads/releases/download/v0.1.0-beta.1/Polyscript-0.1.0-beta.1-mac-arm64.zip)

- Target: Apple Silicon Macs, macOS 15 or later.
- ZIP: 196,920,732 bytes (about 197 MB).
- Signing: ad-hoc; not notarized.
- Physical installation, microphone permissions, and manual accessibility
  qualification remain pending. This is an experimental preview.
- [Installation instructions and checksum](https://script.polymathlabs.xyz/download.html).

The ZIP contains `Polyscript/Polyscript.app`, Electron's `LICENSE` and
`LICENSES.chromium.html`. Native runtime notices, build receipts, and source
archives are included in the application. Model weights are separate explicit
downloads. The installed app needs no separate Node or Homebrew installation.

SHA-256:

```text
97a6ecc436e65b988bef990c89d38e12093f6e40e173dcdf71b4db3414895bd2
```

Run `shasum -a 256 Polyscript-0.1.0-beta.1-mac-arm64.zip` after downloading and
compare with `SHA256SUMS.txt`.

## First use

1. Extract the ZIP and move `Polyscript.app` to Applications.
2. Open it in Finder. If macOS blocks this unnotarized preview and you choose to
   allow it, follow [Apple's opening procedure](https://support.apple.com/guide/mac-help/open-a-mac-app-from-an-unknown-developer-mh40616/mac)
   in System Settings → Privacy & Security → Open Anyway.
3. Explore the clearly labeled synthetic demo. Keyword recall needs no models.
   Install Whisper Tiny explicitly in Settings for audio; the optional search
   and answer models also require explicit downloads.
4. Obtain everyone's permission and a transcript-use agreement before every
   recording or import. Do not use or share transcripts outside that agreement.

Processing runs locally after setup, with no silent cloud fallback. Interview
use is prohibited even with consent. Every detected interview ends processing
and exits the app with no override, resume, or retry. Detection is imperfect.
Review transcription errors; source citations show what the stored transcript
says, not whether speech recognition heard the original conversation correctly.

See [Privacy & use](https://script.polymathlabs.xyz/privacy.html) for storage and
permission details.
