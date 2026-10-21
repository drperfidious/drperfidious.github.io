Annuals ID — iOS Safari build
==========================

Files:
- index.html            Main game
- manifest.webmanifest  Lets Safari/Home Screen treat it like a web app when hosted

Recommended iPhone use:
1. Upload this folder to any static HTTPS host (GitHub Pages, Netlify, Cloudflare Pages, etc.).
2. Open the resulting HTTPS address in Safari on iPhone.
3. Optional: Safari Share menu -> Add to Home Screen.

Why host it instead of opening index.html directly from Files?
The game makes live cross-origin requests to the iNaturalist API and image servers. A normal HTTPS web origin is substantially more reliable on iOS than a local file/Quick Look context.

The game still requires an internet connection for live iNaturalist observations/photos.
