# Build Command Line Instructions

From inside the zmk folder, start the virtual environment .venv,
then navigate to the app subdirectory within zmk (path/zmk/app).

Then run the following to build the boards found within this repository's config folder:

For the right half:
 west build -d build/right -b orca_right -- -DZMK_CONFIG="C:/Users/Hugh/projects/orca-zmk-config"

For the left half:
 west build -d build/left -b orca_left -- -DZMK_CONFIG="C:/Users/Hugh/projects/orca-zmk-config"
