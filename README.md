# Metal Gear Solid 2: Substance PC "HD"

Higher quality assets for Metal Gear Solid 2: Substance for PC. The goal is to maximize the quality of assets that the engine will allow.

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

## Authors

* **Sam/Vega** [UltimateNova1203](https://github.com/UltimateNova1203)

Any [contributors](https://github.com/UltimateNova1203/mgs2-pchd/contributors) can be found here.

## Acknowledgments

* AnonRunzes and Nisto (from HCS64), for the sdt_demux.py script.
* Joy Division, for various MGS/ZOE tools: https://github.com/Joy-Division/tools-mgs
* kellymoen, for the MGDecrypt tool: https://github.com/kellymoen/MGDecrypt
* Turfster, for the Solidus tool.
* VFansss, for the modern PC patch: https://github.com/VFansss/mgs2-v-s-fix
* Bluepoint Games, for the HD Edition.
* Hideo Kojima, for the experience.
