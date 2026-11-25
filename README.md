# UpScalVids

Independent Python 3.11+ OpenAI Skill, by Sam.

The lightweight Skill ZIP is video2x-video.zip.
Its unpacked source lives in video2x-video/ (see SKILL.md and references/RUNTIME.md).
These are source distributions, not a promise of cloud GPU/installation access.

## Native dependencies (NOT YET PUBLISHED)
Native binaries and model weights are NOT in Git history or the light ZIP.
They must be published separately as release assets after complete licence review.
Each downloader refuses missing releases and checks SHA256 before extraction.

- ffmpeg-windows-x64-2025-02-13.zip; bytes=130661781; sha256=684fc9adee65ff4d0adaf5c269d00be490403e0e68938c6e0974fe31ae51a945
- video2x-ncnn-windows-x64-6.4.0.zip; bytes=204746873; sha256=70dcdc11913453826b728b3639817b105d5242f8cd8ee57a4ee4780d171e8a58

Redistribution of upstream FFmpeg, Upscayl, Video2X, bundled DLLs, models and weight files
requires third-party licence verification and relevant notices/source obligations.
The project source licence is not assigned yet; no implied third-party licence granted.

## Validation
Tested on MINIPC Python 3.11.9; remote ChatGPT Skill runtime not yet validated.
No credential, Cassandre file, private user media, or Windows executable is tracked.

## GitHub release distribution

The heavy native dependencies are attached to the versioned GitHub Release in this repository only. Every download URL and SHA-256 in video2x-video/references/dependencies.json must point to this repository. See the actual Release assets and documented supported platform matrix; Windows binaries do not run on Linux or macOS.

## Téléchargements vérifiés

Les distributions sont séparées pour ce dépôt :

- [Skill Python OpenAI v1.0.2](https://github.com/SamSamantha1977/UpScalVids/releases/download/v1.0.2/video2x-video.zip)
- [Dépendances natives Windows x64](https://github.com/SamSamantha1977/UpScalVids/releases/tag/deps-v1.0.0)
- Manifeste avec URL et empreintes SHA-256 : [dependencies.json](video2x-video/references/dependencies.json)

Les modules natifs tiers conservent leurs propres licences. Voir [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md).
Pour un environnement ChatGPT Linux, les exécutables Windows ne sont **pas** utilisables ; la skill recherche d'abord les logiciels présents dans l'environnement.
