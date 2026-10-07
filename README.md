# NOVA Media Hub

Static-first cinematic media hub designed for GitHub Pages and jsDelivr.

## Included
- Anime discovery/details using AniList GraphQL.
- Movie discovery/details using TMDB v3 (API key entered locally).
- Game discovery/details using RAWG (API key entered locally).
- Local Snake + 2048 arcade.
- Browser-style iframe launcher for sites that allow embedding, plus official external launch buttons.
- AI launchers and a local prompt scratchpad.
- Interactive particle/cursor background.
- Lazy-loaded images, no ad scripts, no analytics, no third-party ad SDKs.
- Authorized MP4/HLS-compatible player shell for media you own or are authorized to play.

## GitHub Pages / jsDelivr
Put these files in a repository root and enable GitHub Pages. The project needs no server-side runtime. jsDelivr can serve the repository files after they are public.

GitHub Pages is static hosting. It cannot safely become a full general-purpose browser/proxy by itself, and many sites block iframe embedding with CSP/X-Frame-Options.

## Important limits
- This project intentionally does **not** implement a censorship/network-filter bypass, Scramjet/Ultraviolet proxy, or access-control circumvention.
- A browser cannot make an iframe/video URL impossible to inspect. Client-side anti-inspect tricks are deterrents only, not security.
- For real media protection, use server-side authorization, short-lived signed URLs, tokenized playback, or DRM where appropriate.
- Do not commit TMDB/RAWG keys to a public repository. This build stores them in localStorage instead.
- Only use media and embeds you have permission to use.

## API notes
TMDB: https://developer.themoviedb.org/docs/getting-started
RAWG: https://rawg.io/apidocs
AniList: https://anilist.gitbook.io/anilist-apiv2-docs
