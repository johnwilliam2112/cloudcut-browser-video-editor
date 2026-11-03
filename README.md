CloudCut – Browser Video Editor

A powerful, mobile-friendly, browser-based video editor powered by Cloudflare Workers and FFmpeg.wasm.

CloudCut lets you edit videos directly in your browser without installing desktop software. Video processing runs locally in the browser.

✨ Features

Video Editing

- Trim and cut videos
- Merge multiple videos
- Resize and crop videos
- Rotate and flip videos
- Change video speed
- Adjust brightness, contrast and saturation
- Apply video effects
- Add text overlays
- Add image watermarks
- Add subtitles

Audio Editing

- Remove or replace audio
- Mix audio tracks
- Normalize audio
- Fade audio in and out
- Export audio separately

Supported Formats

Type| Formats
Video| MP4, WebM, MKV
Audio| MP3, WAV
Animation| GIF
Images| JPG
Subtitles| SRT, ASS, SSA, VTT

Actual codec support depends on the FFmpeg.wasm build.

Export Presets

- YouTube 1080p
- Vertical video (9:16)
- Smaller file size
- GIF export
- MP3 audio export

Other Features

- Mobile-friendly interface
- Multiple media file selection
- English, Persian and Chinese languages
- Browser-based processing
- No server-side video storage

---

🚀 Deploy to Cloudflare

Deploy your own CloudCut instance to Cloudflare Workers with one click.

""Deploy to Cloudflare" (https://deploy.workers.cloudflare.com/button)" (https://deploy.workers.cloudflare.com/?url=https://github.com/johnwilliam2112/cloudcut-browser-video-editor)

1. Click the Deploy to Cloudflare button.
2. Sign in to your Cloudflare account.
3. Connect your GitHub account if requested.
4. Configure your Worker.
5. Deploy!

Each user gets their own independent Cloudflare Worker deployment.

---

🛠 Manual Installation

You can also deploy CloudCut manually.

Option 1 – Cloudflare Dashboard

1. Open "Cloudflare Dashboard" (https://dash.cloudflare.com/).
2. Navigate to Workers & Pages.
3. Create a new Worker.
4. Open the code editor.
5. Copy the contents of "worker.js".
6. Replace the default Worker code.
7. Save and deploy.

Option 2 – Wrangler CLI

Clone the repository:

git clone https://github.com/johnwilliam2112/cloudcut-browser-video-editor.git

Enter the project directory:

cd cloudcut-browser-video-editor

Create "wrangler.jsonc":

{
  "name": "cloudcut-browser-video-editor",
  "main": "worker.js",
  "compatibility_date": "2026-11-02"
}

Deploy:

npx wrangler deploy

---

⚙️ Technology

- Cloudflare Workers
- HTML5
- CSS3
- JavaScript
- FFmpeg.wasm
- Web APIs

No Node.js application server or server-side video processing is required.

🔒 Privacy

CloudCut is designed to process selected media files locally in the user's browser.

- Selected media files are not uploaded to the Cloudflare Worker for processing.
- The Worker serves the web application.
- FFmpeg.wasm and other runtime assets are loaded from external CDNs.
- Processing happens on the user's device.

⚠️ Requirements and Limitations

- A modern browser is recommended.
- An internet connection is required to load external FFmpeg.wasm assets.
- Large video files may require considerable device memory.
- Processing speed depends on the user's device and browser.
- Some codecs and operations depend on the FFmpeg.wasm build.
- Keep the browser tab open during processing and exporting.

📂 Repository Structure

cloudcut-browser-video-editor/
│
├── worker.js
├── wrangler.jsonc
└── README.md

📜 License

No open-source license has currently been specified.

Unless a license is added, all rights are reserved by the repository owner.

---

CloudCut – Edit videos anywhere, directly in your browser.

Made with ❤️ using Cloudflare Workers and FFmpeg.wasm.

"GitHub Repository" (https://github.com/johnwilliam2112/cloudcut-browser-video-editor)
