# Yapfast Enhanced Marketplace

This repository is the public plugin catalog for Yapfast Enhanced. It includes the pinned Ping example and Favorite GIF Folders.

Plugin authors can propose a listing under `plugins/` and add its ID to `index.json`. Include the plugin's HTTPS repository URL, immutable commit, module SHA-256, exact permissions, and license. GitHub and Codeberg plugin repositories can both be listed here.

A listing's **Reviewed** status applies to its exact pinned source commit and module hash. Every new or updated pin requires a source/permission review and successful verification before publication. Review is not a guarantee of safety. See [the Favorite GIF Folders review](reviews/io.github.dmor-me.favorite-gif-folders-1.0.0.md) for its checks and limitations.

The Marketplace reads this catalog when browsing. It shows the plugin and its permissions before installation. Existing installations added by URL retain their source; they are not silently replaced by publishing a listing.

Use a compatible Enhanced plugin helper to check a listing:

```text
yapfast-plugins verify-entry plugins/io.github.dmor-me.favorite-gif-folders.json
```

Registry icons belong under `icons/`: 128×128 WebP, at most 24 KiB. The app can read listing metadata and icons without contacting individual plugin repositories until installation.

Favorite GIF Folders requires an Enhanced host with native media-browser API v1, favorite-GIF access, and JSON file choosers.
