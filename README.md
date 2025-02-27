# Flycast 1.0
![flycast logo](https://github.com/flyinghead/flycast/raw/master/shell/linux/flycast.png)

**Flycast** is a multi-platform Sega Dreamcast, Naomi and Atomiswave emulator derived from [**reicast**](https://reicast.com/).

## Disclaimer

All code contritbuted to this fork is *not* bound by the Individual Contributor License Agreement of the upstream repository (https://github.com/reicast/reicast-emulator) and shall *not* be considered as a contribution to the upstream repository.

## Building for the Trimui Smart Pro

Use the 64-bit ARM docker image seen [here](https://portmaster.games/docker.html) (monkeyx/retro_builder:arm64)

After running and pushing the files to the docker, build the CMakeFiles with the BUILD_TSP tag on. As in:

`cmake -DBUILD_TSP=ON -B build_tsp -S .`

Then run:

`cmake --build build_tsp -j 12`

Replacing "12" with whatever amount of cores your processor has.