# Build Command Line Instructions

From inside the zmk folder, start the virtual environment .venv,
then navigate to the app subdirectory within zmk (path/zmk/app).

Then run the following to build the boards found within this repository's config folder:

For the right half:
 west build -d build/right -b orca_right -- -DZMK_CONFIG="C:/Users/Hugh/projects/orca-zmk-config"
# Linux (Arch) (without ZMK Studio Support)
west build -p -d build/right -b orca_right -- -DZMK_CONFIG="/home/hug/projects/zmk-configs/orca-zmk-config" -DZMK_EXTRA_MODULES="/home/hug/projects/zmk-configs/zmk-includes"
For the left half:
# Windows
west build -d build/left -b orca_left -- -DZMK_CONFIG="C:/Users/Hugh/projects/orca-zmk-config"
# Linux (Arch) (without ZMK Studio Support)
west build -p -d build/left -b orca_left -- -DZMK_CONFIG="/home/hug/projects/zmk-configs/orca-zmk-config" -DZMK_EXTRA_MODULES="/home/hug/projects/zmk-configs/zmk-includes"
## EXTERNAL MODULES

This config requires the following ext modules:

- zmk-helpers
- zmk-includes

If you wish to build with the zmk-helpers module (or any other module),append the following to your west build command: -DZMK_EXTRA_MODULES="C:/Users/hughr/projects/MODULE", change the path as necessary.
