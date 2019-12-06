# Metal Gear Solid 2: Substance PC "HD"

Higher quality assets for Metal Gear Solid 2: Substance for PC. The goal is to maximize the quality of assets that the engine will allow. I'd like to put something here. Excuse me, Hirano-san.

## Getting Started

### Important Notice

Please note that the compiled assets (.\mgs2-pchd\cdrom.img) are not the resolution as the source files (.\mgs2-pchd\source). This is a limitation with the game engine, the game will lock if some assets are too large, such as in resolution (FMVs), total used filesize (textures), etc. There seems to be a max of 64MB-128MB the game will address. Dummying out some assets that we don't see helps to reclaim some (KBs) space. There's a line we have to draw between super crisp HD textures and a usable game. Thus, not everything will be upscaled.

### Installing

Ensure you have a backup in order to revert.

Run the PowerShell script, or extract the ZIP somewhere comfortable and follow below steps.
 
    .mgs2s                  # Game install path
    ├── bin                 # Game EXE and VFansss launcher
    ├── backup              # Recommended location for your backup
    ├── cdrom.img           # Original assets folder
    │   ├── face            # Codec asset folder
	│   ├── pac             # FMV asset folder
    │   └── stage           # Stage asset folder
    └── mgs2-pchd           # HD Pack folder
        ├── cdrom.img       # Compiled assets folder
        └── source          # Source assets folder

Drag and drop the CDROM.IMG folder from MGS2-PCHD over the top of the install path's CDROM.IMG folder.

### Uninstalling

Run the PowerShell script, or restore your backup.

## Methodology

The idea here is to try to get as crisp and clean of assets as we can. Either by cleaning up existing textures, upscaling/downscaling FMVs with cleanup, recapturing FMVs, ripping from the HD/PS2 versions, etc.

### Text

Text was upscaled 4x using nearest neighbor. This is to get the box font to look extra crisp. From there, manual pixel interpolation was done to ensure a consistent and crisp look. As for other text, they have been recreated with a matching font (see [MISC.md](https://github.com/UltimateNova1203/mgs2-pchd/blob/master/MISC.md)).

### Textures

Textures are ripped from the HD Edition or PS2 version, upscaled by hand, or upscaled using waifu2x. If there is any color banding, it was manually touched up by hand to fix it as best as possible.

The upscaling takes the original resolution and upscales it by 4x, so a 256x256 texture will become 1024x1024, 1024x1024 will become 4096x4096, etc. Currently, there is no way to actually load these textures, so the textures then get downsampled by half, so we now have a texture path of 256x256 > 1024x1024 > 512x512, or 1024x1024 > 4096x4096 > 2048x2048, etc. This will preserve the quality while actually (possibly) being able to be used by the game engine.

### Videos

Same as previous, FMVs are ripped from the HD Edition where it made sense. For some FMVs, the HD Edition is no better than what shipped with the PC version. These are either recaptured where possible, touched up by hand, or upscaled with waifu2x.

## Authors

* **Sam/Vega** [UltimateNova1203](https://github.com/UltimateNova1203)

Any [contributors](https://github.com/UltimateNova1203/mgs2-pchd/contributors) can be found here.

## Acknowledgments

* AnonRunzes and Nisto (from HCS64), for the sdt_demux.py script.
* Bluepoint Games, for the HD Edition.
* Hideo Kojima, for the experience.
* Joy Division, for various MGS/ZOE tools: https://github.com/Joy-Division/tools-mgs
* kellymoen, for the MGDecrypt tool: https://github.com/kellymoen/MGDecrypt
* Turfster/LionheartUK/TheDyingInformant, for the Solidus tool.
* VFansss, for the modern PC patch: https://github.com/VFansss/mgs2-v-s-fix
