# keetv2 releases

Release builds of keetv2 for Windows. This repository holds no source code: the workflow checks out
the private keetv2 and MacUIKit repositories with read-only deploy keys, builds on a GitHub-hosted
Windows runner, and attaches `Setup.exe` and the portable zip to a draft release.
