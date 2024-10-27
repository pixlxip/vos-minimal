# Unofficial Vanilla OS Minimal Image

Containerfile for building a minimal Vanilla OS image.

This image is based on top of [`vanillaos/core`](https://github.com/Vanilla-OS/core-image/pkgs/container/core) and offers a minimal
Vanilla OS experience without GNOME.

## Build

> [!NOTE]
> The fsguard compiled plugin `.so` file should be downloaded from the [latest release](https://github.com/Vanilla-OS/vib-fsguard/releases/latest) and be placed under a `plugins` directory beside the `recipe.yml` file.

```bash
vib build recipe.yml
podman image build -t pixlxip/vos-minimal .
```
