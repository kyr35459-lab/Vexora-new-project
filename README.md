# VEXORA STUDIO AI

Static website package prepared for Vercel deployment.

## Deploy to Vercel
1. Upload this folder's contents to a GitHub repository (the `index.html` file must be at the repository root).
2. Import the repository into Vercel.
3. Set Framework Preset to `Other`.
4. Leave Build Command empty (or use no build step).
5. Set Output Directory to `.` if Vercel asks for one.
6. Deploy.

No `package.json` is required for this static HTML version.

## Important feature limitations
This supplied HTML contains a browser-side photo/video editor using Canvas, WebCodecs where supported, and a MediaRecorder fallback. Its prompt interpretation is local/deterministic; the supplied file does not contain a Gemini/other AI API integration or a remote AI video-generation backend. Saved project settings use browser localStorage and are not cloud-synced. The MediaRecorder fallback may export WebM rather than MP4 depending on browser codec support.

Do not add secret API keys to this HTML file. A real AI generation integration requires a secure backend and provider credentials stored server-side.
