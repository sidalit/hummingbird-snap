<div align="center">

<img src="snap/gui/hummingbird.png" alt="Hummingbird logo" width="128" />

# Hummingbird

**A native music player for your local library.**

[![hummingbird](https://snapcraft.io/hummingbird/badge.svg)](https://snapcraft.io/hummingbird)
[![Base: core26](https://img.shields.io/badge/Base-core26-2C8C3C?logo=canonical&logoColor=white)](https://snapcraft.io/core26)
![Confinement: strict](https://img.shields.io/badge/Confinement-strict-2C8C3C)
[![Maintainer: sidaliteir](https://img.shields.io/badge/Maintainer-sidaliteir-2C8C3C?logo=snapcraft&logoColor=white)](https://snapcraft.io/publisher/sidaliteir)
![Architectures: amd64 and arm64](https://img.shields.io/badge/Architectures-amd64%20%7C%20arm64-2C8C3C?logo=linux&logoColor=white)

[Getting Started](#getting-started) · [Configure](#configure) · [Limitations](#limitations) · [Build](#build) · [Support](#support) · [License](#license)

Unofficial snap packaging for [Hummingbird](https://git.mailliw.org/hummingbird/hummingbird), a music player with playlists, lyrics and customizable themes.

</div>

---

## Getting Started

<a href="https://snapcraft.io/hummingbird"><img alt="Get it from the Snap Store" src="https://snapcraft.io/en/dark/install.svg" width="180"></a>

```bash
sudo snap install hummingbird
hummingbird
```

Open Hummingbird from your application menu and add your music folders in its settings.

## Configure

Manage your library and preferences in the app. There are no `snap set` options.

| Optional access | Command |
| --- | --- |
| Music on removable storage | `sudo snap connect hummingbird:removable-media` |

Last.fm requires your own API credentials, supplied as `LASTFM_API_KEY` and `LASTFM_API_SECRET` when launching Hummingbird.

## Limitations

- Discord presence is unavailable under strict confinement.
- Audio uses your desktop sound server; direct hardware output is not exposed.
- Application updates are managed by snapd.

## Build

```bash
git clone https://github.com/sidalit/hummingbird-snap.git
cd hummingbird-snap
sudo snap install snapcraft --classic
snapcraft pack
```

## Support

- **Installation or snap issues:** [open a packaging issue](https://github.com/sidalit/hummingbird-snap/issues).
- **Application bugs:** [report them upstream](https://git.mailliw.org/hummingbird/hummingbird/issues).

## License

Snap packaging: [MIT](https://github.com/sidalit/hummingbird-snap/blob/main/LICENSE).
