# Folio downloads

Folio is a reading app for EPUB books, PDFs and audiobooks, with reading and listening kept in sync.
This repository only holds the downloads and the files the apps use to update themselves; the source code is private.

## Windows

Download **Folio-Setup-x.y.z.exe** from the [windows release](https://github.com/eyuelseyoum97/folio-releases/releases/tag/windows) and run it.
Folio then updates itself: it downloads new versions in the background and installs them when you restart or close it.

## Android

Download **Folio-x.y.z.apk** from the [android release](https://github.com/eyuelseyoum97/folio-releases/releases/tag/android) and open it on your phone
(Android asks you to allow installing apps from your browser or file manager). After that, Folio checks for updates itself
(Settings › Check for updates) and Android asks you to confirm each one.

## How updates are protected

Every update carries a signature (the `.sig` file for Windows, `sig` in `latest-android.json` for Android) made with a private key
that never leaves the developer's computer. Both apps check that signature against the installer's SHA-256 before installing anything,
so a changed or fake file is refused even if it were uploaded here.
