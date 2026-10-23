# melodies.

A private, offline-friendly MP3 player that lives in your browser and installs on your home screen like a real app. No accounts, no ads, no tracking. Your music stays on your device.

It's a single web page, so there's nothing to download from an app store.

## Features

- **Play your own MP3s:** add songs from your device and they're saved inside the app
- **Library, Favorites, Playlists, and Queue** tabs
- **Search** your songs by name
- **Favorites:** tap the heart on any song
- **Playlists:** create, rename, and delete them; add songs from inside a playlist (**+ Add songs to this playlist**) or from any song's ⋯ menu
- **Play next and Add to queue:** build a queue on the fly
- **Drag to reorder** songs in the Library, a playlist, or the Queue (grab the ≡ handle)
- **Rename songs:** fix a song's displayed name from its ⋯ menu
- **Shuffle and repeat:** repeat cycles through off, repeat all, and repeat one
- **Playback speed:** 0.75×, 1×, 1.25×, 1.5×, and 2×
- **Picks up where you left off:** remembers your last song and position
- **Remembers your settings:** repeat, shuffle, speed, and theme stick after you close the app
- **Lock screen controls:** play, pause, next, and previous from the lock screen and Control Center, where your device supports it
- **Themes:** Dark (default), Cream, Peach, Mint, and Deep Teal, using the Sweet Summer color palette. The opening screen follows your theme too
- **Opening screen:** a splash with the "m." logo that matches your theme

## Install it on your device

Open the app's web address in your browser first, then follow the steps for your device.

### iPhone and iPad (Safari)

1. Open the app's link in **Safari**. Installing only works from Safari on iOS.
2. Tap the **Share** button.
3. Scroll down and tap **Add to Home Screen**, then tap **Add**.
4. Open **melodies.** from your home screen.

This is the main way the app is designed to be used.

### Android (Chrome)

1. Open the app's link in **Chrome**.
2. Tap the **⋮** menu.
3. Tap **Install app** (or **Add to Home screen**).

### Computer (Chrome, Edge, or Safari)

- **Chrome or Edge:** click the install icon at the right end of the address bar, or open the browser menu and choose **Install melodies.**
- **Safari on Mac:** choose **File → Add to Dock**.

You can also use it without installing, just by keeping the page open in a browser tab.

## Using it

### Adding music

1. In the **Library** tab, tap **Add songs from this phone**.
2. Pick one or more audio files, such as MP3s, from your Files app or wherever they're stored.
3. They appear in your Library. Tap a song to play it.

Tip: if your music is in iCloud Drive, you can pick it straight from there. Songs are copied into the app, so you only need to add each one once per device.

### Playing

- Tap a song to play it. When it ends, the next song in that list plays automatically. If the list runs out, playback carries on down your Library.
- Use the ring and seek bar to jump around in a song.
- The speed button (for example, **1×**) cycles through the playback speeds.
- The heart under the controls favorites the current song.

### Song options (⋯)

Tap the ⋯ next to any song for:

- **Play next:** put it at the front of the queue
- **Add to queue:** put it at the end of the queue
- **Add to playlist…:** add it to an existing playlist or a new one
- **Rename:** change the name shown in the app
- **Remove from this playlist:** only when you're inside a playlist
- **Remove from library:** delete it from the app

Renaming only changes the name shown in melodies. Your original files are never touched. Removing a song deletes only the copy stored inside the app.

### Changing the theme

Tap the half-filled circle at the top right and choose a theme. Your choice is remembered.

## Good to know

- **Your library is stored on each device separately.** Songs, favorites, playlists, and your queue don't sync between devices. If you use melodies. on two devices, you'll need to add your songs to each one.
- **The data lives in your browser's storage.** Clearing website data for the site, or deleting and reinstalling the app on some devices, can erase your library. Keep your original MP3s somewhere safe.
- **It works offline.** After the first visit, the app opens without an internet connection, and your saved songs play offline.
- **Background playback can vary.** Music keeps playing when you lock your phone, but how reliably it behaves depends on your device and browser. iPhone is the most-tested setup.
- **Which files work:** the app plays any audio format your browser can play. MP3 is the safest choice.

## Updating and troubleshooting

- **The app looks old after an update:** fully close it (swipe it away from the app switcher) and open it again.
- **Still not updating:** deleting the app from your home screen and adding it again usually works, but on iPhone it also erases the songs, playlists, and favorites saved inside the app. Only do this as a last resort, and keep your original files handy.
- **The launch screen looks outdated:** iPhone saves launch images when an app is added, so only a freshly added copy picks up new ones.
- **Launch screen color:** the brief screen iPhone shows before the app loads is a fixed black image. Once the app loads, the opening splash uses your theme.
- **Matching the home screen icon to a theme:** an installed app's icon is fixed when it's added, so it can't change by itself. To get a themed icon, open the app's web address in **Safari** (not the home screen app), choose a theme with the button at the top right, then use **Add to Home Screen**. It's a separate copy with its own library, and deleting the old copy erases its saved songs.
- **A song won't play:** the file may be in a format your browser can't play. Try converting it to MP3.
- **Music stops at the end of the list:** turn on repeat all (tap the repeat button until you see "Repeat all").

## What's inside

There's no build step or server. The app is a few static files:

| File | What it does |
| --- | --- |
| `index.html` | The whole app: layout, styling, and logic |
| `sw.js` | Service worker that makes the app work offline |
| `manifest.webmanifest` | Lets the app be installed with a name and icon |
| `icon-*.png` | App icons |
| `splash-*.png` | iPhone launch screen images |

It uses standard browser features: IndexedDB and localStorage for saving your data, the Media Session API for lock screen controls, and a service worker for offline use.

## Credits

- **Wordmark font:** [Yang Bagus](https://www.fontspace.com/yang-bagus-font-f124972) by Khurasan Type, embedded in the app. It's listed as free for personal and commercial use.
- **Themes:** based on the Sweet Summer color palette (Color Palette #06) by KDesign.co.
