
file(GLOB TEMP_SRC *.cpp)
# 不要这个文件
file(GLOB RemoveItems NFCPluginActor.cpp)
list(REMOVE_ITEM TEMP_SRC ${RemoveItems})
add_executable(NFPluginLoader ${TEMP_SRC})
target_link_libraries(NFPluginLoader dl pthread Theron)
