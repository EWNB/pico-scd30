add_library(pico_scd30
    scd30_i2c.c
    sensirion_common.c
    sensirion_i2c_hal.c
    sensirion_i2c.c
)

target_link_libraries(pico_scd30
    hardware_i2c
    pico_stdlib
)

target_include_directories (pico_scd30 PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})
