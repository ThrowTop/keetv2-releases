# keetv2

Peer-to-peer voice, chat, infinite file sharing and high quality screen sharing for Windows.

![A voice call in a group](screenshots/call.png)

## Why

- **Low latency voice.** In our tests keetv2 arrives over 200 ms ahead of Discord and about 90 ms
  ahead of TeamSpeak on the same sound.
- **Native.** C++ and Retained Qt with Direct3D 11. Not Electron slop.
- **No servers.** Peers connect directly and every connection is encrypted. Your account lives on
  your devices.
- **Screen sharing on your GPU.** NVENC, AMF or Quick Sync, H.264, HEVC or AV1, up to 120 fps.
- **Everything is a setting.** Codec, bitrate, noise suppression, encoder, latency. (Including some you probably shouldnt touch unless you know what you are doing)
- **Familiar.** Laid out like Discord, looks like a Mac app.

Not vibe-coded slop. Every part was built and measured with care: SIMD with compiler
intrinsics for the hot paths, no allocations on the audio thread for minimal latency, raw bytes for media between
processes.

| | |
|---|---|
| ![Voice processing settings](screenshots/voice-processing.png) | ![Screen sharing settings](screenshots/screen-sharing.png) |

![Voice input and output settings](screenshots/voice-devices.png)

## Install

Download `keetv2-desktop-win-Setup.exe` from the [latest release](../../releases/latest) and run
it. No administrator rights needed. keetv2 updates itself (can be disabled in settings).

Windows 10 or 11, x64.

## Why closed source

To keep the code from being scraped to train AI models.
