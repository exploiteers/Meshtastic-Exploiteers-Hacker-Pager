# This file was automatically generated for projects
# without default 'CMakeLists.txt' file.

# Note: several directories for other device types are deliberately not included below:
# "src/platform/nrf52" "src/platform/stm32wl" "src/platform/rp2xx0" "src/mesh/eth" "src/mesh/raspihttp"
FILE(GLOB src_norecurse
    ${CMAKE_SOURCE_DIR}/src/*.*
    ${CMAKE_SOURCE_DIR}/src/mesh/*.*
)

FILE(GLOB_RECURSE src_recurse 
    ${CMAKE_SOURCE_DIR}/src/buzz/*.*
    ${CMAKE_SOURCE_DIR}/src/concurrency/*.*
    ${CMAKE_SOURCE_DIR}/src/detect/*.*
    ${CMAKE_SOURCE_DIR}/src/Fusion/*.*
    ${CMAKE_SOURCE_DIR}/src/gps/*.*
    ${CMAKE_SOURCE_DIR}/src/graphics/*.*
    ${CMAKE_SOURCE_DIR}/src/input/*.*
    ${CMAKE_SOURCE_DIR}/src/mesh/api/*.*
    ${CMAKE_SOURCE_DIR}/src/mesh/compression/*.*
    ${CMAKE_SOURCE_DIR}/src/mesh/generated/*.*
    ${CMAKE_SOURCE_DIR}/src/mesh/http/*.*
    ${CMAKE_SOURCE_DIR}/src/mesh/wifi/*.*
    ${CMAKE_SOURCE_DIR}/src/modules/*.*
    ${CMAKE_SOURCE_DIR}/src/motion/*.*
    ${CMAKE_SOURCE_DIR}/src/mqtt/*.*
    ${CMAKE_SOURCE_DIR}/src/nimble/*.*
    ${CMAKE_SOURCE_DIR}/src/platform/esp32/*.*
    ${CMAKE_SOURCE_DIR}/src/power/*.*
    ${CMAKE_SOURCE_DIR}/src/serialization/*.*
)

idf_component_register(
    SRCS ${src_norecurse} ${src_recurse}
)
