# radio-dashboard

A one-page radio dashboard with big buttons. Your stations, one tap, no apps, no ads.

Free. Take it, fork it, make it yours.

## What it is

One HTML file with your favorite radio stations as big tap targets. Hit a station, it plays instantly. Hit it again, it stops. That's the whole app.

It uses the stations' direct stream URLs, so there's no ad-loaded web player in the way — audio starts immediately.

## Use it

No build, no dependencies, no server needed.

1. Open `index.html` in any browser, or host it anywhere static (GitHub Pages works).
2. On your phone: open the page in Chrome (Android) or Safari (iPhone) → **Add to Home Screen**. It installs as a standalone app with its own icon.
3. Tap a station. Done.

## Make it yours

The example ships with three stations. Swap in your own — one block per station in `index.html`:

```html
<button class="station" data-stream="YOUR_DIRECT_STREAM_URL" data-name="Station Name">
  <div class="freq"><span class="dot"></span>101.1 Name</div>
  <div class="name">City &middot; Genre</div>
</button>
```

You need the station's **direct stream URL** (usually an MP3 or AAC stream), not the web player page. Most stations publish one; check their website's source or a stream directory like [streamtheworld](https://www.streamtheworld.com) or your broadcaster's streaming host.

## Files

- `index.html` — the whole app
- `manifest.webmanifest` — home-screen install metadata
- `icon-192.png`, `icon-512.png` — app icons (replace with your own)

## License

Public domain. Do whatever you want with it.
