---
layout: default
title: KiwiWire privacy policy
---

[Home](./) · [KiwiWire](./kiwiwire.html) · [Privacy](./kiwiwire-privacy.html) · [Support](./kiwiwire-support.html)

## KiwiWire privacy policy

**Effective date:** September 22, 2026

This policy describes the KiwiWire Android app, a podcast player created and owned by Ethan Stidley.

**Developer:** Ethan Stidley

**Contact:** [estidley@gmail.com](mailto:estidley@gmail.com)

### The app

KiwiWire is a local-only podcast player. There is no KiwiWire account. There is no KiwiWire backend or server. KiwiWire does not sync the library to the cloud.

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

This data stays on the device. KiwiWire does not upload it to a KiwiWire server.

### Network

When you add a feed, or play or download an episode, KiwiWire sends HTTPS requests to the podcast publisher host you chose. Those requests fetch the RSS feed, the episode file (enclosure), and artwork.

The User-Agent is `KiwiWire/1.0`.

KiwiWire does not include an analytics SDK, an advertising SDK, or a crash-reporting SDK.

### Tips

Optional tips use Google Play Billing. Google processes the payment. KiwiWire does not collect card numbers.

### Cast, Wear, and Play services

If you use Cast, Wear, or other Google Play services features, those features run through Google Play services. KiwiWire uses them when you use those features.

### Permissions

- `INTERNET` — fetch feeds, episode audio, and artwork from the publisher host you chose
- `ACCESS_NETWORK_STATE` — check whether the device has a network connection
- `FOREGROUND_SERVICE` / `MEDIA_PLAYBACK` — keep playback running with a foreground service while audio plays
- `POST_NOTIFICATIONS` — show playback and download notifications

WorkManager, used for background work such as downloads, may also use `WAKE_LOCK` and `RECEIVE_BOOT_COMPLETED` through its libraries.

### Backup

Android backup and device transfer are off for this app (`allowBackup=false`). The KiwiWire library is not included in Google backup or device transfer.

### Deleting data

You can clear the library in the app (Clear library, or the equivalent control). Uninstalling KiwiWire removes the app’s private data from the device.

KiwiWire has no accounts, so there is no account-deletion page.

### Changes

This policy may be updated on this page. The effective date above will change when it is updated.
