# Thumbnail specification notes

## What the official pages state

The CSV keeps the source URL beside each value so a reader can re-check the current wording. The video-thumbnail page covers the recommended canvas, 16:9 ratio, minimum width, listed formats, upload limits, and Shorts guidance. The channel-branding page covers the banner canvas, safe area, TV recommendation, and file-size limit.

## What is intentionally not filled in

The official help pages used for this reference do not publish a fixed pixel-by-pixel crop map for standard thumbnails across phone, desktop, and TV. They also do not state a banner file-format list on the channel-branding page. This reference leaves those fields out instead of inventing values.

## CDN observations

The thumbnail URL builder uses the direct image path observed in the live browser test:

```text
https://i.ytimg.com/vi/{video_id}/{filename}
```

The CSV records only the five filenames that loaded for the tested video. A browser tool should check whether each requested image actually loads before presenting it as available.
