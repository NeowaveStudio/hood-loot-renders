# Hood Loot renders

Cinematic clips for Hood Loot, served from Render's CDN as a static site. The game reads
`/active.json` → `/<set>/manifest.json` → `/<set>/<screen>/<clip>`.

- Sets are **write-once**: clips are cached `immutable` for a year, so a new delivery is a new set.
- Build a set from the game repo: `pnpm renders:cdn --set 2026-09-16a --out ../hood-loot-renders --activate`,
  then commit and push here. Only `active.json` changes for existing sets.

© the Hood Loot project. These files are served publicly to players; they are not licensed for reuse.
