
file(GLOB TEMP_SRC *.cpp)
list(REMOVE_ITEM TEMP_SRC .*NFCPluginActor.cpp)
list(LENGTH TEMP_SRC SRC_LEN) 
message(STATUS ${SRC_LEN})
add_executable(NFPluginLoader ${TEMP_SRC})
