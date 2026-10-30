# SS IPTV remote nested playlist proof of concept

Test for VIDAA / SS IPTV hierarchical playlist navigation using **public demo streams only**.

No HydraTV account information, password, or private IPTV links are included.

## SS IPTV external playlist URL

`https://cdn.jsdelivr.net/gh/ameeter/github-slideshow@ssiptv-nested-poc/ssiptv-nested-poc/index.m3u`

Fallback raw GitHub URL:

`https://raw.githubusercontent.com/ameeter/github-slideshow/ssiptv-nested-poc/ssiptv-nested-poc/index.m3u`

## Expected on the TV
* Open **Nested Test**
* Select **Live TV** -> **Sports (Test Category)** -> one of two demo channels -> play
* Or select **Movies** -> **Sample Movie - Mux Demo** -> play

This validates remote M3U retrieval and nested playlist navigation only. It does not validate HydraTV or its credentials.

The root and sub-playlists use the officially documented SS IPTV `#EXTINF:0 type="playlist"` convention.
