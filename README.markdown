# Oh My Scrobbles

Oh My Scrobbles adds your listening from this Mac's Apple Music app to your Last.fm profile. It lives in the menu bar, shows what's playing, and keeps a library window with your scrobble history, loved tracks, Rewind and Friends.

**[Download for Mac](https://github.com/robbyrussell/oh-my-scrobbles-releases/releases/latest/download/OhMyScrobbles.dmg)** · [What's new](CHANGELOG.markdown) · [Previous releases](https://github.com/robbyrussell/oh-my-scrobbles-releases/releases) · [Report a problem](https://github.com/robbyrussell/oh-my-scrobbles-releases/issues/new/choose)

> Oh My Scrobbles is in early beta. Updates are delivered directly for now, and we're exploring the Mac App Store for the future.

## Screenshots

### The Menubar 

<img width="367" height="594" alt="image" src="https://github.com/user-attachments/assets/80c49861-d0ca-4596-a467-39e5586fa87a" /> <img width="379" height="946" alt="image" src="https://github.com/user-attachments/assets/1a83f41b-6518-4497-8748-74485d07b59b" />

### The Essentials

<img width="1086" height="1245" alt="image" src="https://github.com/user-attachments/assets/2fda00d0-a6d2-46db-8146-960ac53aac61" />

View your scrobble history

<img width="1086" height="1245" alt="image" src="https://github.com/user-attachments/assets/8006692d-01c1-421e-abbf-550023999f74" />

View your loved tracks

### Rewind

A bunch of fun tools to allow you to reconnect with your past listening habits. Find stuff you've not heard in ages!

<img width="942" height="1236" alt="image" src="https://github.com/user-attachments/assets/f2173353-dbc0-4ef6-97b7-5a9de351b20e" />

<img width="1080" height="734" alt="image" src="https://github.com/user-attachments/assets/3774681a-67c9-45ee-8cbb-64eed26680df" />

<img width="936" height="1017" alt="image" src="https://github.com/user-attachments/assets/f818fe25-86ff-4a11-9e97-0a19d489a9d2" />

### Settings / Preferences

<img width="912" height="1128" alt="image" src="https://github.com/user-attachments/assets/88614497-b027-41f5-9cfa-1246e9ab8e84" />

Yes, it kind of works with Apple Radio, too!

<img width="913" height="734" alt="image" src="https://github.com/user-attachments/assets/67ed93ae-11b1-485b-ab5a-2cdf7f885e99" />

Sync! Yes, you can sync all of your Last.fm scrobbling history to your local computer. This speeds up our tool and gives you some fun access options.

<img width="1003" height="861" alt="image" src="https://github.com/user-attachments/assets/bb0a7d86-cc11-49df-89cd-259b33035264" />

..did we mention Themes? Robby likes a good theme. 

<img width="1003" height="861" alt="image" src="https://github.com/user-attachments/assets/cc5380e7-1531-4473-9836-f0a923bf0796" />

Cache controls...

### Artists / Albums

Browse albums and see some of your own stats, where applicable.

<img width="1086" height="1245" alt="image" src="https://github.com/user-attachments/assets/66d8d892-5b1b-4249-9854-88234c2deb6c" />

<img width="1086" height="1245" alt="image" src="https://github.com/user-attachments/assets/a4e8d7b2-f283-4850-9a3c-21439be52605" />

### Friends

Keep up with what your friends (who you're following on Last.fm) last scrobbled.

<img width="1086" height="1245" alt="image" src="https://github.com/user-attachments/assets/52a304c5-55de-45f9-8aac-54b7219d2641" />



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
