# Metal Gear Solid 2: Substance PC "HD"

Higher quality assets for Metal Gear Solid 2: Substance for PC. The goal is to maximize the quality of assets that the engine will allow. I'd like to put something here. Excuse me, Hirano-san.

## Methodology

The idea here is to try to get as crisp and clean of assets as we can. Either by cleaning up existing textures, upscaling/downscaling FMVs with cleanup, recapturing FMVs, ripping from the HD/PS2 versions, etc.

### Text

Text was upscaled 4x using nearest neighbor. This is to get the square font to look extra crispy. From there, manual pixel interpolation was done to ensure a consistent and crisp look. As for other text, they have been recreated with a matching font (see [MISC.md](https://github.com/UltimateNova1203/mgs2-pchd/blob/master/MISC.md)).

### Textures

Textures are ripped from the HD Edition or PS2 version, upscaled by hand, upscaled using waifu2x, etc. If there is any color banding, it was manually touched up by hand to fix it as best as possible.

The upscaling takes the original resolution and upscales it by 4x, so a 256x256 texture will become 1024x1024, 1024x1024 will become 4096x4096, etc. Currently, there is no way to actually load these textures.

### Videos

Same as previous, FMVs are ripped from the HD Edition where it made sense. For some FMVs, the HD Edition is no better than what shipped with the PC version. These are either recaptured where possible, touched up by hand, or upscaled.

## Authors

* **Samantha** [UltimateNova1203](https://github.com/UltimateNova1203)
* **Michelle** [TachiCola](https://github.com/TachiCola)

Any [contributors](https://github.com/UltimateNova1203/mgs2-pchd/contributors) can be found here.

## Acknowledgments

* AnonRunzes and Nisto (from HCS64), for the sdt_demux.py script: https://hcs64.com/mboard/forum.php?showthread=46911
* Bluepoint Games, for the HD Edition.
* fnord software, for the DDS plug-in: https://fnordware.blogspot.com/2014/09/dds-plug-in-for-after-effects-and.html
* gdkchan, for MilkGear: https://github.com/LeonamMiiller/MilkGear
* Hideo Kojima, for the experience.
* Joy Division, for various MGS/ZOE tools: https://github.com/Joy-Division/tools-mgs
* kellymoen, for the MGDecrypt tool: https://github.com/kellymoen/MGDecrypt
* TachiCola, for assistance with file formatting and tools: https://github.com/tachicola/pkgrip
* Turfster, for the Solidus tool.
* VFansss, for the modern PC patch: https://github.com/VFansss/mgs2-v-s-fix
