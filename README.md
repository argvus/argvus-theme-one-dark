# One Dark theme for ARGVUS

Official ARGVUS Dark theme, `one-dark`, with its Sticky and Float variants.

[![CI](https://github.com/argvus/argvus-theme-one-dark/actions/workflows/ci.yml/badge.svg)](https://github.com/argvus/argvus-theme-one-dark/actions/workflows/ci.yml)
[![Release](https://github.com/argvus/argvus-theme-one-dark/actions/workflows/release.yml/badge.svg)](https://github.com/argvus/argvus-theme-one-dark/actions/workflows/release.yml)
[![License](https://img.shields.io/badge/License-GPL--3.0-blue.svg)](LICENSE)

## Theme identity

| Field | Value |
| --- | --- |
| Theme ID | `one-dark` (Float variant: `one-dark-float`) |
| Display name | One Dark |
| Mode | `dark` |
| Default highlight | `#61AFEF` |
| GTK color scheme | `prefer-dark` |
| Calendar stylesheet | `one-dark` |
| Package | `argvus-theme-one-dark` |
| Wallpaper | `/usr/share/backgrounds/argvus/abstract/dark/one-dark-abstract-dark.jxl` |

The values above are the ones declared in
`src/usr/share/argvus/appearance/themes.d/one-dark/theme.toml`, the manifest that the
desktop reads. The manifest is the source of truth; this page describes it.

## Installing

The package depends on `argvus` and `argvus-appearance`, so pacman installs them with it.

```sh
sudo pacman -S argvus-theme-one-dark
```

Select the theme in the Control Center (Appearance > Themes), or run
`argvus theme-switch one-dark`.

## Files

The package installs the theme's per-component files under `/usr/share/argvus` (and the
calendar stylesheet under `/etc/argvus/taskbar/calendar/themes`). Each component that
the theme styles has its own directory, listed by `find src -type f` in this repository.

## Development

Validate with `make validate` before building. The design rules are in
[DEVELOPMENT.md](DEVELOPMENT.md); the ARGVUS documentation for themes is in
`argvus/docs/en/user-guide/appearance.md` of the `argvus` repository.

## License

GPL-3.0-only. See [LICENSE](LICENSE).
