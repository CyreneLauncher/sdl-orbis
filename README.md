# sdl-orbis

SDL 3 with the Orbis threading adaptations and a virtual PS4 gamepad, built as the `libSDL3`
PRX that Controlify loads at run time. See PORT-PROVENANCE.json for exact origins; its
`upstream` record is the pinned SDL release this recipe builds.

```sh
python3 build_sdl3.py --sdk /path/to/ps4-payload-sdk --toolchain /path/to/PS4Toolchain --fetch
```

Inputs: `orbis-runtime-support` as a sibling checkout, or `ORBIS_RUNTIME_SUPPORT`.
`ORBIS_BUILD_ROOT` (default `build/`) holds `downloads/` and the output in `sdl3/`.
The launcher sets it to its `graphics-probe/build`. This repository does not depend on LWJGL.
