---
layout: default
title: KiwiWire privacy policy
---

[Home](./) · [KiwiWire](./kiwiwire.html) · [Privacy](./kiwiwire-privacy.html) · [Legal](./kiwiwire-legal.html) · [Support](./kiwiwire-support.html)

## KiwiWire privacy policy

**Effective date:** October 8, 2026

This policy describes the KiwiWire Android app, a podcast player created and owned by Ethan Stidley.

**Developer:** Ethan Stidley

**Contact:** [estidley@gmail.com](mailto:estidley@gmail.com)

### The app

KiwiWire is a podcast player with a library stored on your device. There is no KiwiWire account or KiwiWire backend. KiwiWire does not operate a cloud library-sync service. Android backup and device transfer may copy eligible app data as described below.

### Data on the device

KiwiWire stores the following on the device, in app-private storage (a Room database named `kiwiwire.db`, plus downloaded episode files):

- Subscriptions and RSS feed URLs
- Episode metadata
- Listen progress
- Bookmarks
- Up Next
- Smart rules
- Playback settings
- Downloaded episode files

KiwiWire does not upload this library to a KiwiWire server or to the podcast directory. Android backup, device transfer, and exports are described below.

### Network

When you add a feed, or play or download an episode, KiwiWire sends HTTPS requests to the podcast publisher host you chose. Those requests fetch the RSS feed, the episode file (enclosure), and artwork.

Podcast hosts and artwork hosts receive the requests needed to deliver their content, including the requested URL, your connection's IP address, and ordinary HTTP request information. Their own privacy policies apply.

### Podcast discovery and Apple

Discover uses the Apple Podcasts catalog through the iTunes Search API and related directory endpoints. Opening Discover requests categories and charts for the selected region. Searching sends your search terms and selected region to Apple. Apple receives your connection's IP address and ordinary request information. RSS URLs pasted into the feed input are processed as feed subscriptions rather than directory search terms.

KiwiWire does not send your saved library, listening history, bookmarks, or downloaded audio to Apple's directory. Discovery results are cached locally to reduce requests and support previously viewed results while offline. Those cache files are excluded from Android backups and library JSON exports. Your selected region is saved in app preferences.

Directory artwork is requested from the artwork host returned by Apple. After subscription, feeds, artwork, and audio are requested from the podcast publishers or their hosting providers. These hosts may receive your IP address and request information.

Choosing the Listen on Apple Podcasts badge opens that show's Apple page in your browser or an available app. The badge graphic itself is included in KiwiWire and does not make a separate network request. Apple's services are governed by [Apple's privacy policy](https://www.apple.com/legal/privacy/). See our [legal and third-party notices](./kiwiwire-legal.html) for provider and trademark information.

KiwiWire does not include an analytics SDK, an advertising SDK, or a crash-reporting SDK.

### Tips

Optional tips use Google Play Billing. Google processes the payment. KiwiWire does not collect card numbers.

### Cast, Wear, and Play services

If you use Cast, Wear, or other Google Play services features, those features run through Google Play services. KiwiWire uses them when you use those features.

### Permissions

- `INTERNET` — fetch directory results, feeds, episode audio, and artwork from their providers
- `ACCESS_NETWORK_STATE` / `ACCESS_WIFI_STATE` — check connectivity and Wi-Fi availability for download preferences and playback
- `FOREGROUND_SERVICE` / `FOREGROUND_SERVICE_MEDIA_PLAYBACK` / `FOREGROUND_SERVICE_DATA_SYNC` — keep user-started playback and downloads running with visible notifications
- `POST_NOTIFICATIONS` — show playback and download notifications

WorkManager, used for background work such as downloads, may also use `WAKE_LOCK` and `RECEIVE_BOOT_COMPLETED` through its libraries.

### Backup

Current versions allow Android to back up the library database and app preferences, subject to your device's backup settings and backup provider. These data may also be included in Android device transfer. Downloaded audio and directory cache files are not included by KiwiWire's backup rules.

Export library as JSON creates a file in the location you choose. That file can contain feed URLs, subscriptions, listening progress, bookmarks, queue entries, and settings. Audio files are not included. You control sharing and deletion of exported files; clearing the app does not delete copies you saved elsewhere.

### Deleting data

You can clear the library in the app (Clear library, or the equivalent control). Uninstalling KiwiWire removes the app’s private data from the device.

KiwiWire has no accounts, so there is no account-deletion page.

### Changes

This policy may be updated on this page. The effective date above will change when it is updated.
