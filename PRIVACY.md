# Privacy Policy — Weather Dashboard+

**Last updated: August 29, 2026**

Weather Dashboard+ ("the app") is made by Joe Page. This policy covers the Android, iOS, macOS,
Windows and Linux versions.

The short version: **there is no account, no advertising, and no third-party analytics or tracking
SDK.** Your locations and settings live on your device. The app talks to weather services to fetch a
forecast.

---

## What stays on your device

Everything you configure: your saved locations, which weather source you use and any API key you
entered for it, units, card order, icon set, and every other setting. These are stored in the
platform's normal settings store (Android `SharedPreferences`, iOS `UserDefaults`, and a file under
`~/.weather-dashboard/` on desktop). None of it is uploaded, and deleting the app removes it.

Weather responses and background photos are also cached on the device so the screen isn't blank when
the network drops.

---

## Location

The app needs a location to show a forecast for it — that's the whole function of the app. There are
three ways it gets one, and you control which:

- **A city you add by name.** Nothing about your device is involved; you searched for it.
- **Device location (GPS).** On Android and iOS, only if you grant location permission, and only
  while the app is open. The app never requests background location.
- **A rough location from your IP address.** Used when you have declined or revoked location
  permission, when no GPS fix is available, and always on desktop — desktop has no GPS. This resolves
  to roughly your city, not your address, via [ipwho.is](https://ipwho.is).

Whichever way it's obtained, the location is used to fetch weather, radar, pollen and a matching
background photo, and it is stored on your device. **It is never sent to the developer, and it is
never included in the anonymous usage counts described below.**

Location permission is optional. Decline it and the app still works — add cities by name, or let it
fall back to the IP-based lookup.

---

## Services the app contacts

The app is a client for public weather services. When it fetches data, that service necessarily
receives the coordinates being requested and your device's IP address, and each one handles that
under its own privacy policy.

| Service | What it receives | When |
|---|---|---|
| [Open-Meteo](https://open-meteo.com/en/terms) | Coordinates | Every forecast refresh (the default source). Also city-name searches, and air quality where it's the pollen source |
| [Visual Crossing](https://www.visualcrossing.com/privacy-policy/) | Coordinates, your API key | Only if you select it as your weather source |
| [OpenWeatherMap](https://openweather.co.uk/privacy-policy) | Coordinates, your API key | Only if you select it as your weather source |
| [Unsplash](https://unsplash.com/privacy) | A search term for the current sky condition (e.g. "rain"), not your location | While photo backgrounds are enabled |
| [Iowa State University Mesonet](https://mesonet.agron.iastate.edu/) + Esri / OpenStreetMap | The map area you're viewing | While the radar card is on screen |
| [pollen.com](https://www.pollen.com/privacy) | A US ZIP code | While the pollen card is on screen, in the US |
| [US Census geocoder](https://www.census.gov/privacy) | Coordinates | To turn a location into the ZIP code pollen.com needs |
| [Google Pollen](https://policies.google.com/privacy) | Coordinates, your API key | Only if you add a Google Pollen key |
| [GitHub](https://docs.github.com/site-policy/privacy-policies/github-general-privacy-statement) | Nothing but the request itself | Update checks — **sideloaded Android and desktop only.** App Store and Play Store builds never do this |

The developer does not receive a copy of any of these requests.

---

## What the app never does

- No advertising, ad network, or ad ID.
- No third-party analytics, attribution, or tracking SDK.
- No account, sign-in, or email collection.
- No selling or sharing of data with anyone, for any purpose.
- No background location, and no location reported to the developer.

---

## Children

The app isn't directed at children, and it doesn't knowingly collect anything from them. It has no
account system and collects no personal information from anyone.

---

## Your choices, in one place

| To do this | Go here |
|---|---|
| Stop using device location | Revoke location permission in the OS, or remove "Current Location" from your list |
| Stop contacting Unsplash | Settings ▸ Background ▸ Image Source — pick the bundled photos or gradients |
| Remove everything stored locally | Uninstall the app (desktop: delete `~/.weather-dashboard/`) |
| Have a support report or crash log deleted | Email the address below |

---

## Contact

Questions, or a deletion request: **joe.page.software@gmail.com**, or open an issue at
[github.com/jpage4500/WeatherDashboardPlus](https://github.com/jpage4500/WeatherDashboardPlus/issues).
