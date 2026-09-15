# Weather Dashboard+ — Support

Weather Dashboard+ is a full-screen weather app built for a tablet left on a wall, a counter or a
desk. This page is where to get help with it.

---

## Ask a question or report a problem

**Email [joe.page.software@gmail.com](mailto:joe.page.software@gmail.com)** — no account needed, and
questions, bug reports and feature requests are all welcome. It's one developer answering, so expect
a reply within a couple of days.

Tell me which device you're on and what you were doing when it went wrong and I can usually work it
out from there. The fastest route is the app's own report, which attaches the logs for you:

> Open the **☰** menu at the top left ▸ **About** ▸ **Support / Feedback** — type what happened and
> send. The app attaches its recent log file so I can see the error rather than guess at it.

---

## Getting started

- **Nothing to sign up for.** There's no account and no API key. The default weather source
  (Open-Meteo) is free and keyless, so the app works the moment it opens.
- **Tap or scroll up on the main screen** to reveal the hourly strip, the daily forecast, the radar,
  pollen and the details. Scroll back down and you're left with the photo and the temperature again.
- **Add a location** with the **+** button at the top right — search by city name, or add your
  current location. Swipe left and right to move between them.
- **Everything else** is behind the **☰** menu at the top left: **Settings** and **About**.

---

## Common questions

### It says "Current Location" but shows the wrong place

The app asks for location permission the first time it needs it. If you declined, it falls back to a
rough position worked out from your internet connection, which is usually the right region but can be
the wrong city — and on a desktop computer that's the only thing available.

To fix it, either grant location permission in your device's system settings, or ignore "Current
Location" entirely and add your city by name with the **+** button.

### No weather is showing, or it can't reach the weather service

Almost always the network. Pull down on the main screen to retry.

If it keeps failing, check **Settings ▸ Weather ▸ Weather Source**. Visual Crossing and
OpenWeatherMap need an API key you supply yourself, and a mistyped or expired key looks exactly like
an outage. Switching back to **Open-Meteo** rules that out, since it needs no key.

### The temperature is in the wrong units

**Settings ▸ Weather ▸ Use Celsius.** Wind speed, pressure and visibility all follow that one switch.

### The screen keeps turning off on my wall tablet

**Settings ▸ Display ▸ Dashboard Mode.** That's the setting that keeps the screen awake, and it can
also dim, blank or screensaver it overnight instead of leaving a bright panel in a dark room. The
device needs to be plugged in and the app needs to be in the foreground.

One thing worth knowing on an iPad: once the screen has actually slept, nothing in an app can wake it
again. So a scheduled "off" period works best dimmed or blanked rather than truly asleep —
[there's a page about the workarounds here](docs/public/ios-wake.md).

### The radar card isn't there

Radar covers **the United States only**, and the card is hidden for locations outside it rather than
shown empty. **Settings ▸ Weather ▸ Radar Source** names the coverage for each choice.

### Pollen is empty, or says it has no data

Coverage depends on the source, under **Settings ▸ Weather ▸ Pollen Source**:

| Source | Coverage | Key needed |
|---|---|---|
| Automatic (default) | picks the best free source for each location | no |
| Pollen.com | US only | no |
| Open-Meteo | Europe only | no |
| Google Pollen | worldwide | yes |

If your area isn't covered by any of the free sources, a Google Pollen key is the only way to fill
that card in.

### Can I use my own photos as the background?

Yes — **Settings ▸ Background ▸ Image Source ▸ My Photos**, then add photos with the **My Photos**
row that appears under it. They're copied into the app from your device's photo picker and are never
uploaded anywhere.

The same screen is the way out of online photography entirely: **Built-in** uses the images that ship
with the app, and **Gradient** uses no photos at all.

### How do I make it refresh more often?

**Settings ▸ Weather ▸ Refresh Interval** — 10 minutes by default. You can always pull down on the
main screen for an immediate refresh.

---

## Privacy and your data

The app has no account, no ads and no tracking. What it does collect, why, and how to have anything
deleted is written out in full in the
[privacy policy](https://github.com/jpage4500/WeatherDashboardPlus/blob/main/PRIVACY.md).

To request deletion of a support report or crash log, email the address above.

---

## Something else

If your question isn't here, just ask —
**[joe.page.software@gmail.com](mailto:joe.page.software@gmail.com)**.
