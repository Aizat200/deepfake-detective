# DeepFake Detective — Interactive Digital Media Verification Simulator

A React + Tailwind CSS educational prototype for the FTSM Simulator Challenge. Users investigate **three fictional cases**: a fake investment broadcast, an emergency voice note, and a campus announcement. Includes a dashboard, case library, evidence inspection lab, branching decisions, learning feedback, and browser-local progress tracking.

## Run locally

Requirements: Node.js 18+

```bash
npm install
npm run dev
```

Open the local URL shown by Vite (usually http://localhost:5173).

## Production build

```bash
npm run build
npm run preview
```

Deploy the generated `dist/` folder to any static hosting service. Vite uses a relative base path (`./`) so GitHub Pages project hosting works.

## GitHub Pages

1. Push the repository to GitHub.
2. Run `npm install && npm run build`.
3. Deploy `dist/` with GitHub Actions (configure Pages source as GitHub Actions) or an equivalent static deployment workflow.

## Important educational limitations

- Cases and findings are fictional and **do not contain actual video/audio deepfake samples**. The media panel is a simulated placeholder; its playback controls demonstrate UI state only.
- This prototype **does not detect deepfakes** and does not compute authenticity probabilities.
- Missing metadata or odd visual artifacts are **not proof** of AI generation.
- Progress is saved to the browser's localStorage; no personal information or uploaded media is sent to a server.
- AI-generated media detection and live uploads are deliberately out of scope for this MVP.

## Recommended next steps

Add properly licensed, clearly labeled sample media; implement real frame-by-frame navigation and Web Audio waveform inspection; include a pre/post learning assessment; validate case conclusions with a subject expert; and perform usability testing.

## Reference resources

- NIST: https://www.nist.gov/publications/reducing-risks-posed-synthetic-content-overview-technical-approaches-digital-content
- C2PA: https://c2pa.org/

## Version 2 — functional multimedia lab
The `/public/media` folder includes fictional, locally generated educational media: an investment training video with synthetic narration, a synthetic emergency voice recording, and a fictional campus notice. The Evidence Lab has functional HTML5 video/audio playback, adjustable playback speed, timeline scrubbing, 0.2-second seeking, video frame snapshots, audio waveform rendering and a campus-source comparison. These are synthetic *training examples*, not real-world verified deepfakes or a machine-learning detection engine. No real individual's likeness or voice is impersonated.
