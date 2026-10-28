# Verification

Final source: Flow candidate 4, upscaled within Flow to 1920x1080 at 24fps. Compared contact sheets against 720p original: consistent geometry, ascent and cloud motion; no conspicuous new artifacts. This is an upscale, not native 1080p.

Desktop/mobile layout checked in Chrome at 1440x960, 1920x1080, 900x700, 768x1024, 390x844 and 375x812: no horizontal overflow. Mobile feature blocks do not overlap. Actual forward/reverse seeking, poster loading and recorder endpoint were checked. Local HTTP Range returns 206. Final encoded media verified with ffprobe: H.264/yuv420p, 24fps, 121 frames, no audio, faststart, keyframes every four frames.

Limitations: reduced-motion and Save-Data branches are implemented but not device-emulated. Google Fonts requires network access. AI media can contain minor synthetic texture artifacts. Fictional testimonials are labelled.
