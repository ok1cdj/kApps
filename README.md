# kApps — Apps for the Mudita Kompakt

Landing page for a small family of free, open-source Android apps built for the
[Mudita Kompakt](https://mudita.com/) e-ink phone. Every app is designed around
e-ink from the first line of code — no Google Services, no background services,
no tracking in the apps.

The site is a single static `index.html` (plus screenshots) and is published
with GitHub Pages. Release versions and APK download links are fetched live from
the GitHub Releases API at page load.

## The apps

| App | What it does |
|-----|--------------|
| [kRadar](https://github.com/ok1cdj/kRadar) | Precipitation radar (RainViewer over an offline vector map, quantised for e-ink). |
| [kCompass](https://github.com/ok1cdj/kCompass) | GPS, compass and Maidenhead locator, fully offline. |
| [kZivyobraz](https://github.com/ok1cdj/kZivyobraz) | Client for the [zivyobraz.eu](https://zivyobraz.eu) e-paper service. |
| [kSread](https://github.com/ok1cdj/kSread) | Speed reader (RSVP) — one word at a time, no scrolling. |
| [kChat](https://github.com/ok1cdj/kchat) | Client for OpenAI-compatible chat endpoints, bring your own key. |
| [kVexed](https://github.com/ok1cdj/kVexed) | The classic Vexed sliding-block puzzle, offline and permission-free. |

## Installing an app

Download the APK from the app's Releases page and open it on the phone, or push
it over ADB with `adb install`. To get updates automatically, add the app's
GitHub repository to [Obtainium](https://github.com/ImranR98/Obtainium).

## Developing the page

It's plain HTML/CSS/JS with no build step. Serve it locally with:

```
python3 -m http.server 8000
```

then open <http://localhost:8000>. Screenshots live in `screenshots/` and are
named after each repo in lowercase (e.g. `kradar.png`).

## Author

Ondřej Koloničný — [GitHub](https://github.com/ok1cdj)

## License

The apps are released under their own licenses (mostly GPL); see each
repository. This page is free to reuse.
