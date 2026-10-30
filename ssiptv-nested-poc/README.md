# HydraTV catalog validation — actual records from IPTV Smarters

This GitHub test now contains **real HydraTV names and content identifiers**, extracted from the IPTV Smarters Android HAR capture of October 30, 2026. All sample videos were removed.

## Load on SS IPTV

https://raw.githubusercontent.com/ameeter/github-slideshow/ssiptv-nested-poc/ssiptv-nested-poc/index.m3u

### Actual captured subset

- Live TV: BeIN Sport 4K, BeIN Sport HD, NEWS (5 real channels per group)
- Movies: 2026 English, 2025 English, Cinema Hydra (5 real movies per group)
- Series: NetFlix → Away → Season 1 (10 real episodes)

This is a limited static **40-item validation subset**, not the full provider catalog (11,380 live channels, 32,059 movies, 15,601 series at capture).

**CRITICAL SECURITY LIMITATION:** This repository is public. All playback URLs intentionally contain placeholder segments `YOUR_USERNAME/YOUR_PASSWORD` instead of your real credentials. Browsing real category names and titles works; **playing content from these public GitHub playlists will not work without replacing those placeholders in a private copy**. Never commit account credentials, device keys, full HAR files, or personalized stream links to a public branch.

To validate video, use a private M3U file with your credentials and upload it through SS IPTV My Playlist rather than publishing it.

A complete remote playlist with automatic updates and authenticated streams requires a private gateway (not implemented in this PoC).

The provider's API uses `POST player_api.php` to fetch catalogs; direct media URLs under `/live`, `/movie`, `/series` require authentication.
