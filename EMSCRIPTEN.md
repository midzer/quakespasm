# Emscripten

## Build

```
cd Quake
emmake make
```

## Link

```
emcc -fno-rtti -fno-exceptions -flto=thin -O3 *.o libGL.a -o index.html -lGL -sFULL_ES2 -sMAX_WEBGL_VERSION=2 -sUSE_SDL=2 -sUSE_MODPLUG -sASYNCIFY -sINITIAL_MEMORY=320mb --preload-file id1/ --closure 1
```
