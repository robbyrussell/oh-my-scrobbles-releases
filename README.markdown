# Oh My Scrobbles

Oh My Scrobbles adds your listening from this Mac's Music app to your Last.fm profile. It lives in the menu bar, shows what's playing, and keeps a library window with your scrobble history, loved tracks, Rewind and Friends.

**[Download for Mac](https://github.com/robbyrussell/oh-my-scrobbles-releases/releases/latest/download/OhMyScrobbles.dmg)** · [What's new](CHANGELOG.markdown) · [Previous releases](https://github.com/robbyrussell/oh-my-scrobbles-releases/releases) · [Report a problem](https://github.com/robbyrussell/oh-my-scrobbles-releases/issues/new/choose)

> Oh My Scrobbles is in early beta. Updates are delivered directly for now, and we're exploring the Mac App Store for the future.

## Screenshots

<!--
Screenshot slots. Each image must be a capture of the real, running app, checked for private
details (account names, friends, avatars, listening you'd rather not share) before it is added.
Put the PNGs in assets/screenshots/ with these names, then remove the comment markers around
each line. Keep the alt text and captions; they describe what the image shows for people who
can't see it.

![The Oh My Scrobbles menu bar panel showing the song playing in Music, its progress and the Last.fm connection](assets/screenshots/menu-bar-panel.png)
*The menu bar panel: what's playing in Music, and whether it's being scrobbled.*

![The Listening Library window showing recent scrobbles in History](assets/screenshots/library-history.png)
*History in the library window: your recent scrobbles from Last.fm.*

![Settings, General, showing the Last.fm account, Scrobbling and Updates sections](assets/screenshots/settings-updates.png)
*Settings: your Last.fm connection, scrobbling, and how often to check for updates.*
-->

Screenshots of the running app are on their way.

## What it does

- Reads the song playing in the Music app on this Mac and scrobbles it to Last.fm once you've played half of it or four minutes of it, whichever comes first. Songs of 30 seconds or less aren't scrobbled, following Last.fm's rules.
- Counts only playback it actually observed. Pauses, skips ahead and time while your Mac sleeps don't count toward a scrobble.
- Keeps plays queued when you're offline and sends them, in order, once Last.fm can be reached again.
- Only reads the current song. It opens Music or starts a song only when you press Open Music or Play, and it never stops or skips playback.

It works with the Music app on this Mac. It doesn't scrobble from other players, your iPhone or other devices.

## Requirements

- macOS 14 Sonoma or later.
- Tested on Apple silicon Macs. The app is universal, but it hasn't been tried on an Intel Mac yet.
- A Last.fm account. You don't need Xcode or a Last.fm API key of your own.

## Install

1. Download **[OhMyScrobbles.dmg](https://github.com/robbyrussell/oh-my-scrobbles-releases/releases/latest/download/OhMyScrobbles.dmg)**.
2. Open it and drag **Oh My Scrobbles** to the **Applications** folder.
3. Eject the disk image, then open Oh My Scrobbles from your Applications folder. If macOS says it was downloaded from the internet, choose **Open**.

Open it from Applications, not from the disk image or your Downloads folder. A copy opened from there can't update itself or open at login.

## First launch

A setup window walks you through three things:

1. **Music access.** macOS asks whether Oh My Scrobbles may control Music. Choose **Allow**: that's how it reads the current song. If you chose **Don't Allow**, turn it on again in System Settings → Privacy & Security → Automation → Oh My Scrobbles → Music.
2. **Connect Last.fm.** Choose **Connect…**, approve access on the Last.fm page that opens in your browser, then come back to the app. Your Last.fm password never passes through Oh My Scrobbles, and the session is kept in your Mac's Keychain.
3. **Find the menu bar icon.** Click it any time to see what's playing. **Launch at login** is in Settings.

## Updates

Oh My Scrobbles checks for new versions on its own while it's open: **weekly** unless you choose otherwise in **Settings → General → Updates**.

- **Daily**, **Weekly** or **Monthly**: checks once a day, every 7 days or every 30 days. New versions download in the background and install the next time you quit the app. You can turn off **Download and install automatically** to be asked first.
- **Never**: no checks on its own.
- **Check for Updates…** works with any setting, in Settings, in About, and in the app menu.
- **What's New** opens the [changelog](CHANGELOG.markdown).

Updates are signed, and the app checks each signature before installing. Checking doesn't need a GitHub account. Like any web request, an update check shows GitHub your IP address and the app version, and nothing else about your Mac.

To update by hand instead: quit Oh My Scrobbles, download the latest disk image, drag the app to Applications and choose **Replace**, then open it from Applications. Your Last.fm connection, settings and queued plays are kept.

## Report a problem or suggest something

Use **[GitHub Issues](https://github.com/robbyrussell/oh-my-scrobbles-releases/issues/new/choose)**, or choose **Report a Problem** in the app's About window or Settings. It helps to include:

- The version and build, from **About Oh My Scrobbles** (for example `Version 0.1.0 (20261030.01)`).
- Your macOS version, from the Apple menu → About This Mac.
- What happened, what you expected, and the steps that lead to it.

Issues are public. Don't paste your Last.fm password, session details, or anything from your listening history you'd rather keep private.

## Privacy

Oh My Scrobbles talks to Last.fm to scrobble and to show your history, to MusicBrainz, Wikidata and Wikimedia Commons for artist photos, and to this repository to check for updates. It has no analytics or tracking, and update checks send no system profile.

## About

Oh My Scrobbles is an independent project. It is not made, endorsed or sponsored by Apple or Last.fm. Apple, Apple Music, Mac and macOS are trademarks of Apple Inc. Last.fm and AudioScrobbler are trademarks of their respective owner. The app bundles [Sparkle](https://sparkle-project.org) for updates; its license is in the app's About window.
