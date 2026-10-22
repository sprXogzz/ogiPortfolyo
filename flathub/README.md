# My Garage for Linux

My Garage is a Flutter desktop application for tracking vehicles, expenses,
fuel purchases, maintenance plans and vehicle incidents. It supports English
and Turkish, local record storage, JSON backup and restore, and CSV and PDF
reports. Linux reminders are shown inside the application; Linux system
notifications are not supported in this version.

This release contains the precompiled x86_64 Linux application. The application
source code is private. The `.sh` files are desktop integration helpers; the
application runs through the `my_garage` executable and the compiled libraries
in `lib/`.

## Package contents

- `my_garage`: native Linux executable.
- `lib/`: Flutter engine, compiled application and native plugin libraries.
- `data/`: application assets and Flutter runtime data.
- `dev.orahmetsevik.MyGarage.desktop`: desktop menu entry.
- `dev.orahmetsevik.MyGarage.metainfo.xml`: application catalog metadata.
- `dev.orahmetsevik.MyGarage.svg`: application icon supplied by the developer.
- `my-garage-launcher.sh`: launcher for the Flatpak installation paths.
- `my-garage-which.sh`: executable lookup helper used by the file picker.

## Running the native bundle

Keep `my_garage`, `lib/` and `data/` together after extracting the archive.
From that directory, run `./my_garage` without root privileges. A native Linux
desktop needs GTK 3; file selection dialogs also require Zenity on the host.
The Flatpak package supplies its own desktop dependencies and launchers.

## Project and distribution

- Developer: Oğuz Rahmet Şevik.
- Project website: https://orahmetsevik.dev/
- Windows edition: [Garajım - Araç Takip on Microsoft Store](https://apps.microsoft.com/detail/9P1LKTZWC44S).
- Application license: proprietary; see the [terms of use](https://garajim-legal.vercel.app/kullanim-kosullari.html).

The Windows listing identifies the existing Windows edition. It is not a
record of the Linux edition's first release date. Third-party libraries
retain their respective licenses.
