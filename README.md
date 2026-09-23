# freecadcmd

A standalone headless FreeCAD image — FreeCAD from its official release
AppImage (see `Dockerfile`), pinned by release tag and checksum-verified,
plus `potrace` for tracing raster artwork into vector outlines.

```sh
# amd64
docker pull ghcr.io/brhelwig/freecadcmd:latest-amd64
docker run --rm ghcr.io/brhelwig/freecadcmd:latest-amd64 freecadcmd --version

# arm64
docker pull ghcr.io/brhelwig/freecadcmd:latest-arm64
docker run --rm ghcr.io/brhelwig/freecadcmd:latest-arm64 freecadcmd --version
```

Built for `linux/amd64` and `linux/arm64` on every push to `main`, weekly,
and on manual dispatch. Each platform is published under its own tag
(`:latest-amd64`, `:latest-arm64`) rather than a combined multi-arch
manifest — pull the tag matching your host's architecture.
