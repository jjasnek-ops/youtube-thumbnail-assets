# YouTube Thumbnail Assets

A small, dependency-free reference set for building browser tools around YouTube thumbnail files and upload specifications.

## What's here

- `data/youtube-thumbnail-files.csv` — browser-observed thumbnail filenames, URL templates, and natural image dimensions from one real video test.
- `data/youtube-upload-specs.csv` — official upload guidance transcribed from YouTube Help pages, with the source URL kept beside each row.
- `docs/thumbnail-spec-notes.md` — practical notes that separate published guidance from gaps the official pages do not define.
- `tools/thumbnail-url-builder.html` — a no-dependency browser tool that turns a video ID into the tested CDN URL variants.

The dimensions in the thumbnail CSV were read from images loaded in a browser from `i.ytimg.com` for video ID `dQw4w9WgXcQ` on 2026-09-13. They are observations for that test video, not a promise that every video exposes every filename or a substitute for an official YouTube API contract.

For an interactive browser-only downloader and preview workflow, see [Thumbnail Tester](https://feedthumbnail.com/youtube-thumbnail-downloader).

## Use the URL builder

Open `tools/thumbnail-url-builder.html` in a browser, enter a video ID, and select **Build URLs**. The tool only constructs links; it does not upload files or require an account.

## Sources

- [YouTube Studio Help — Add custom thumbnails](https://support.google.com/youtubecreatorstudio/answer/72431?co=GENIE.Platform%3DDesktop&hl=en)
- [YouTube Help — Manage your channel branding](https://support.google.com/youtube/answer/10456525?hl=en)

## License

MIT. See `LICENSE`.
