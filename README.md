# freecadcmd

A standalone headless FreeCAD image — FreeCAD from its official release
AppImage (see `Dockerfile`), pinned by release tag and checksum-verified,
plus `potrace` for tracing raster artwork into vector outlines.

```sh
podman pull ghcr.io/brhelwig/freecadcmd:latest
podman run --rm ghcr.io/brhelwig/freecadcmd:latest freecadcmd --version
```

Built for `linux/amd64` and `linux/arm64` on every push to `main`, weekly,
and on manual dispatch. `:latest` is a multi-arch manifest, so the same tag
pulls the image for your host's architecture.
