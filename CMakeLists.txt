add_library(sdl2gfx
        SDL2_rotozoom.c
        SDL2_framerate.c
        SDL2_framerate.h
        SDL2_gfxPrimitives.c
        SDL2_gfxPrimitives.h
        SDL2_gfxPrimitives_font.h
        SDL2_imageFilter.c
        SDL2_imageFilter.h
        SDL2_rotozoom.h
)

find_package(SDL2 REQUIRED)
include_directories(${SDL2_INCLUDE_DIRS})
target_link_libraries(sdl2gfx ${SDL2_LIBRARIES})