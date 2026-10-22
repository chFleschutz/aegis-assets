# aegis-samples

The sample project of [Aegis Engine](https://github.com/chFleschutz/aegis-engine): the examples' scenes
and the assets they, `aegis-test` and the device tests load. The engine checks it out as the opt-in
submodule `samples/`:

    git submodule update --init --checkout samples

It follows the engine's project layout (`docs/asset-system.md`): every asset lives in `content/`, the only
folder the engine scans, and each source file's `.meta` sidecar is committed with it, because scenes
reference assets by ID. `.aegis/` holds the local cache and is never committed.

- `content/models/` - one folder per model, its files as exported (`basic/` holds simple test meshes)
- `content/materials/` - material files, their textures in `textures/`
- `content/environments/` - HDR skies
- `content/scenes/` - the examples' scenes; stress scenes in `stress/`, `aegis-test`'s in `tests/`
- `screenshots/` - the models' screenshots, linked from their READMEs

## Credits

- [Damaged Helmet](content/models/damaged_helmet/README.md) - ctxwing and theblueturtle_, CC BY 4.0 / CC BY-NC 4.0
- [Metal-Rough Spheres](content/models/metal_rough_spheres/README.md) - Ed Mackey (Analytical Graphics, Inc.), CC BY 4.0
- [SciFi Helmet](content/models/sci_fi_helmet/README.md) - Michael Pavlovic, converted by Norbert Nopper, CC0 1.0
- [Sponza](content/models/sponza/README.md) - Crytek, CRYENGINE Limited License Agreement

The models come from the [Khronos glTF Sample Assets](https://github.com/KhronosGroup/glTF-Sample-Assets);
each folder keeps its `LICENSE.md`.
