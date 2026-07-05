# Football Pulse 2026 Podcast

Static podcast landing page for "足球脉动 2026", a World Cup commentary episode with an embedded audio player and full transcript.

## Live Site

- Production: https://football-pulse-2026-podcast.vercel.app
- GitHub: https://github.com/Martin-Mythos/football-pulse-2026-podcast
- Vercel project: `martin-comet-s-projects/football-pulse-2026-podcast`

## Project Structure

```text
.
├── index.html
└── README.md
```

The page is a single static HTML file. Vercel local metadata and environment files are intentionally ignored by Git.
The Vercel deployment also ignores project documentation and local metadata through `.vercelignore`, so only the static page is published.

## External Dependencies

- Tailwind CSS CDN: `https://cdn.tailwindcss.com`
- Google Fonts CSS: `https://fonts.googleapis.com`
- Audio source: `https://opal.google/board/blobs/5316b3f4-e540-4679-8e1d-eea846cf3175`

The audio is not checked into this repository. Playback depends on the external `opal.google` blob remaining publicly reachable.

## Deploy

```bash
git push
```

The Vercel project is connected to the `Martin-Mythos/football-pulse-2026-podcast` GitHub repository. Pushing to `main` triggers production deployment.

## Verification

Last verified on 2026-07-05:

- Production URL returned `HTTP 200`.
- Deployed page title matched `足球脉动 2026 | 世界杯深度播客`.
- Vercel dry run uploaded only `index.html`; `.env.local`, `.gitignore`, and `.vercel` were ignored.
- External audio URL returned `HTTP/2 200` with `content-type: audio/wav`.
