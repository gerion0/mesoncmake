# Meson-CMake demo project

## Build

with CMake:
```
cd subprojects/app
mkdir build; cd build
cmake .. -GNinja -DSDK="$PWD/../../sdk"
ninja
```

with Meson:
```
meson setup build; cd build
ninja subprojects/app/app
```

## License

All code in this repo is in the public domain.
