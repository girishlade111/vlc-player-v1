# vlc-player-v1 — VLC-Style Video Player UI Drafts (React)

A set of early React component drafts for a **VLC-style video player UI**. These are design/prototype iterations (`.tsx`-style JSX snippets) — not a runnable app, no package.json or build setup. Kept as reference material for the UI exploration that led to later player versions.

## Contents

| File | Lines | Notes |
|------|-------|-------|
| `vlc-player preview 1` | 247 | First pass: basic player layout |
| `vlc-player final preview v1` | 276 | Refined layout |
| `vlc-player final preview v2` | 299 | Lucide icons replaced with custom SVGs |
| `vlc-player final preview v3` | 373 | Most complete: playback-speed control, custom icons |

## Component features (across drafts)

- Custom SVG control icons — Play, Pause, Stop, Skip Forward, Volume, Maximize, Speed, Chevron
- Playback-speed control (`changePlaybackSpeed`)
- Time formatting helper (`formatTime`)
- Playlist model (`VideoFile`: name / file / object URL)
- Built with React hooks: `useState`, `useRef`, `useEffect`

## How to use

These files are raw JSX snippets with no extension. To experiment with one:

1. Rename the file you want, e.g. `vlc-player final preview v3` → `VideoPlayer.tsx`
2. Drop it into any React + TypeScript project
3. Wire the component into your app — it manages playback via a `<video>` element ref

Example:

```tsx
// rename to VideoPlayer.tsx, then:
import { VideoPlayer } from './VideoPlayer';

function App() {
  return <VideoPlayer />;
}
```

> Note: the snippets may reference helper components or styles from the original design sandbox; expect small adjustments when integrating.

## Tech stack

- React (hooks) + TypeScript/JSX
- Custom inline SVG icons (no icon library)
- Vanilla CSS styling (no CSS framework)

## License

See [LICENSE](./LICENSE).

---

Built by [Girish Lade](https://ladestack.in) — part of the [LadeStack](https://ladestack.in) collection.
