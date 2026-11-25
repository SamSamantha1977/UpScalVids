# UpScalVids — dépôt de dépendances exclusivement

Ce dépôt GitHub ne distribue PAS les archives ZIP des skills. Les ZIP légers sont autonomes et fournis séparément.
Ce dépôt contient les dépendances lourdes (GitHub Releases), les manifestes SHA-256 et les références d'origine.

## Moteurs, modèles et distributions

- ffmpeg / windows-x64 : 121652518 octets
  - Téléchargement : https://github.com/SamSamantha1977/UpScalVids/releases/download/deps-v1.0.0/ffmpeg-windows-x64-2025-02-13.zip
  - SHA-256 : 54d99f06e60e16e2f2835eed9c30584e5ddf407ff61e5e7a3a65e5065c67ed5e
- ffmpeg / linux-x64 : 93270996 octets
  - Téléchargement : https://github.com/binmgr/ffmpeg/releases/download/v9.0.2/ffmpeg-linux-amd64.tar.gz
  - SHA-256 : d7a22611c3d6793d2939ff992db8feecfdb9c206a583aa31d9a887e0992502c8
- video2x-ncnn / windows-x64 : 198825927 octets
  - Téléchargement : https://github.com/SamSamantha1977/UpScalVids/releases/download/deps-v1.0.0/video2x-ncnn-windows-x64-6.4.0.zip
  - SHA-256 : dc99dfc0d04a46fd2c3491016afc46781b0f43649be78d11e7c9dc23264ee4f3
- video2x-ncnn / linux-x64 : 231232704 octets
  - Téléchargement : https://github.com/k4yt3x/video2x/releases/download/6.4.0/Video2X-x86_64.AppImage
  - SHA-256 : 8238fc38325107f0a08a140d069baee3db80c5ac7470b0a516cc683183f5f92d

## Licences et limites

Conserver THIRD_PARTY_NOTICES.md et les licences d'origine, notamment les conditions propres aux poids IA.
Les moteurs nécessitent le système/architecture correspondant, les bibliothèques compatibles et parfois un GPU Vulkan.
Les modèles et moteurs Windows ne sont pas exécutables sur Linux. Certains poids IA peuvent être communs aux deux systèmes.
Les poids Upscayl d'origine sont référencés dans UPSTREAMS.md; Real-ESRGAN et RIFE sont inclus dans les archives Video2X.
L'exécution réelle des moteurs Linux doit être validée sur une machine Linux équipée d'un GPU compatible.

## Utilisation par la skill

Au lancement d'un mode nécessitant un moteur absent, la skill télécharge les actifs HTTPS épinglés
dans dependencies.json et valide le SHA-256 avant extraction ou exécution.
La variable SAM_SKILL_AUTO_DOWNLOAD=0 empêche tout téléchargement automatique.
