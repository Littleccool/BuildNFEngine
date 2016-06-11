
file(GLOB TEMP_SRC *.cpp)
file(GLOB RemoveItems NFCPluginActor.cpp)
message(STATUS ${RemoveItems})
list(REMOVE_ITEM TEMP_SRC ${RemoveItems})
list(LENGTH TEMP_SRC SRC_LEN) 
message(STATUS ${SRC_LEN})
add_executable(NFPluginLoader ${TEMP_SRC})
