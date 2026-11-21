# Kyoto sky and river — 2026-11-16

The sky and gravel-bed albedo are original images generated with the built-in OpenAI image_gen tool for this project. They are photographic-looking generated imagery, not photographs of a particular location. The ripple normal is an original periodic, band-limited stochastic height-field derivative prepared inside Blender. Existing PLATEAU / OpenStreetMap stage attribution remains unchanged.

Runtime assets:

- `kyoto-sky.jpg`: 2048×1024 sRGB equirectangular background; normal and high quality.
- `kyoto-sky-lite.jpg`: 1024×512 sRGB background; light quality.
- `kyoto-waterbed.jpg`: 1024×1024 sRGB stationary gravel bed, repeated every 2.6 m.
- `kyoto-waterbed-lite.jpg`: 512×512 sRGB gravel bed; light quality.
- `kyoto-water-normal.png`: 512×512 linear / Non-Color periodic ripple normal; all qualities.

The LDR sky supplies matching reflection colours through a bounded-resolution PMREM. Directional and hemisphere lights provide daylight energy. This is not a generated HDR light probe. River appearance combines a stationary bed, depth-dependent tint, angle-dependent reflection and moving normals. It does not use a fluid simulation, screen-space transmission, or live reflections of the bridge and trees.

Authoring scene: `kyoto-marathon/kyoto-sky-water.blend` in the parent workspace. Original generated images and exact prompts: `kyoto-marathon/work/sky-water-2026-11-16/source/`. Preparation and scene scripts: `kyoto-marathon/tools/{prepare_sky_water,build_sky_water_preview,preview_riverbank_nodes}.py`. Game screenshots, comparison images, video and verification records are in the same work directory. Cycles / AgX differs from the browser renderer; game captures are the final visual reference.
