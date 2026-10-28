# Ocean Freight — Above Everything

Final candidate 4, with Google Flow 1080p upscale. AI-generated concept.

A cinematic, scroll-driven ocean freight concept built with plain HTML, CSS and JavaScript. No framework or build step.

## Run locally

Serve this folder with a static HTTP server, for example `python -m http.server 8080`, then visit http://localhost:8080.

## Interaction

The sticky scene fills the viewport. Text moves naturally over the ship. The video stays paused: scrolling seeks forward or backward through the clip. The first 46% of the clip maps to the final feature leaving the viewport; the remaining 54% maps to another 0.75 viewport.

At widths up to 900px, or with Save-Data enabled, the site loads the 720p version. Larger screens load 1080p. Reduced-motion uses the poster without downloading video. A media failure also falls back to the poster.

Use `?rec=1` for a 6.5-second automated scroll with cubic-bezier(.45,.05,.55,.95). The `window.__recTime(video,tMs)` helper supports deterministic external recording.

## Media and design

The ship illustration and video are AI-generated. The reference was created with the available OpenAI image tool; its precise model version was not reported. Video was generated in Google Flow with Omni 1.1 Flash. The 1080p delivery file is upscaled from the 720p source.

Delivery media: H.264/yuv420p, 24fps, 121 frames (~5.042s), no audio, faststart and a keyframe every four frames. The poster is extracted from the first video frame.

The supplied single-file layout is retained, including Exo 2 and Public Sans typography, mirrored desktop features, single-column mobile layout, and the cream testimonial section. Google Fonts requires a network connection. Testimonials are explicitly fictional demonstration content.

## Deployment

Static hosting; no secrets, API keys or server runtime required. Vercel uses the repository root. See VERIFICATION.md for actual checks and remaining limitations.

