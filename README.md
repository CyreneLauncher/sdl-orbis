# sdl-orbis

Owns the extracted Orbis port sources. See PORT-PROVENANCE.json for exact origins.
History was extracted from orbis-launcher with git subtree; the upstream source
archives and supported profiles remain hash-pinned in lwjgl-orbis.

Build: `python3 build_sdl3.py --help`.
Set `ORBIS_LAUNCHER_ROOT` when the integration checkout is not the default sibling
`orbis-launcher`. The integration supplies the toolchain, shared PRX recipe and
output locations; this repository owns the backend and its build adaptations.
