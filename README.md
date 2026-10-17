# radio-dashboard

A one-page radio dashboard with big buttons. Your stations, one tap, no apps, no ads.

Free. Take it, fork it, make it yours.

## What it is

One HTML file with your favorite radio stations as big tap targets. Hit a station, it plays instantly. Hit it again, it stops. That's the whole app.

It uses the stations' direct stream URLs, so there's no ad-loaded web player in the way — audio starts immediately.

## Get it on your phone (2 minutes)

Opening the downloaded file directly won't work right — the page needs to live on the web so your phone can install it as an app. Easiest free way is GitHub Pages:

1. **Fork this repo** (the Fork button, top right on GitHub).
2. In your fork, go to **Settings → Pages**. Under "Build and deployment", set Source to **Deploy from a branch**, Branch to **main**, then **Save**.
3. Wait about a minute, then open `https://YOUR-USERNAME.github.io/radio-dashboard/` — that's your radio, live on the web.
4. On your phone, open that URL in Chrome (Android) or Safari (iPhone) → menu → **Add to Home Screen**.
5. Tap the new home-screen icon, tap a station. Done.

No build, no dependencies, no server. Any static host works too (Netlify, Cloudflare Pages, your own box) — just upload the files and open the URL on your phone.

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
