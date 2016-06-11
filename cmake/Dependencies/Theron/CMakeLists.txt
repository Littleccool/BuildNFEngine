
include_directories(Include)
file(GLOB TEMP_SRC Theron/*.cpp)
add_library(Theron ${TEMP_SRC})
set_target_properties(Theron PROPERTIES RUNTIME_OUTPUT_DIRECTORY ${DependenciesLibPath})
