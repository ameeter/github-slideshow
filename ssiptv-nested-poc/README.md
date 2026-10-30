# SS IPTV nested playlist proof of concept

Public test assets only. No IPTV provider credentials or subscription links are stored.

## Primary link (GitHub Raw)

https://raw.githubusercontent.com/ameeter/github-slideshow/ssiptv-nested-poc/ssiptv-nested-poc/index.m3u

## Alternate link (jsDelivr CDN)

https://cdn.jsdelivr.net/gh/ameeter/github-slideshow@ssiptv-nested-poc/ssiptv-nested-poc/index-cdn.m3u

The branch `ssiptv-nested-poc` is separate from the repository's default branch.

## Expected TV navigation

**Nested Test** -> **Live TV** -> **Sports (Test Category)** -> **Sample HD Channel - Mux Demo** -> video.

**Nested Test** -> **Movies** -> **Sample Movie - Mux Demo** -> video.

## Notes

Only this test is hosted; it does not access HydraTV. Use SS IPTV **External Playlists**, not an individual channel item. Verify remote URL first in a browser, then validate nested navigation on the TV. If raw-hosted nested playlists fail to load, test the jsDelivr alternate.
