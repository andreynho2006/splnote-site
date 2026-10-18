# splnote-site

Public website for the SPLNOTE iOS app (home, support, privacy policy, terms), ready for GitHub Pages from `main`.

Plain HTML with inline CSS; no build step, JavaScript, or runtime dependencies. All paths are relative so the site can be hosted under a GitHub Pages project path. `.nojekyll` enables direct static hosting.

## Preview

Run `python3 -m http.server 8000` from this folder and open `http://localhost:8000`.

## Publish checklist

1. Set the real App Store URL in the hero badge (`href="#"`) and the app ID in the commented `apple-itunes-app` meta tags.
2. Confirm the public Pages URL. Add canonical and `og:url` tags to each page, and make `og:image` and `twitter:image` absolute URLs. The existing relative image paths are local-preview placeholders.
3. Confirm a public support contact. The existing support and legal copy still directs beta users to Send Beta Feedback in TestFlight. Set the privacy policy’s exact effective date at publication.
4. When authorized, publish this repository on GitHub and select **Settings → Pages → Deploy from a branch → main → / (root)**. Enable HTTPS. No remote or custom domain is configured by this task; there is intentionally no `CNAME`.

## Media and review

See [media/CREDITS.md](media/CREDITS.md) for provenance and Apple badge usage. Screenshots are optimized WebP captures of the Native Calm UI. The icons are simple S wordmarks until an app icon is supplied.

All pages support light/dark system preferences, keyboard navigation, reduced motion, and mobile layouts. Marketing claims follow the supplied feature check. SPLNOTE records payments; it does not transfer money.
