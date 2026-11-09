# keetv2 releases

Windows releases of keetv2. Installed copies update themselves from the published releases here.

This repository holds no source code. Its workflow (run by hand) checks out the private keetv2 and
MacUIKit repositories with read-only deploy keys, builds on a GitHub-hosted Windows runner, and
uploads the Velopack release (`Setup.exe`, full and delta packages, `releases.win.json`) as a draft
or a published release.
