# Third-party distribution notice — UpScalVids

The root MIT LICENSE applies to independently authored Python glue and
documentation only. It does not relicense third-party binaries, models or
libraries.

## Video2X 6.4.0 and libraries
- Source release: https://github.com/k4yt3x/video2x/releases/tag/6.4.0
- Source repository: https://github.com/k4yt3x/video2x
- Upstream license: GNU Affero General Public License v3.
- Upstream NOTICE: https://github.com/k4yt3x/video2x/blob/master/NOTICE
- NCNN: https://github.com/Tencent/ncnn (BSD 3-Clause)
- Real-ESRGAN NCNN: https://github.com/xinntao/Real-ESRGAN-ncnn-vulkan
- RIFE NCNN: https://github.com/nihui/rife-ncnn-vulkan
- Real-CUGAN: https://github.com/nihui/realcugan-ncnn-vulkan
- The original Video2X DLL bundle and AI models are subject to the
  corresponding upstream notices and license requirements. The bundled
  original Video2X copyright/license is in LICENSE_VIDEO2X.txt.

## FFmpeg and FFprobe
- FFmpeg: https://ffmpeg.org
- Windows full build: gyan.dev, 2025-02-13, revision 19a2d26177.
- Statically linked GPLv3 build, and Video2X also includes FFmpeg DLLs.
- https://www.gyan.dev/ffmpeg/builds/
- https://ffmpeg.org/legal.html
- https://github.com/FFmpeg/FFmpeg/tree/19a2d26177
- Redistribution requires proper source availability and license notices.

## Usage limits
- FFmpeg interpolation is not RIFE AI.
- All packaged native components target Windows x64 only.
- ChatGPT Linux container without GPU/Vulkan cannot run native Windows
  Video2X engine.
