cmake_minimum_required(VERSION 2.8)

project(NoahFrame)
set(SolutionDir ${PROJECT_SOURCE_DIR})
message(STATUS "SolutionDir=" ${SolutionDir})
include_directories(
${SolutionDir}
${SolutionDir}/Dependencies/ 
${SolutionDir}/Dependencies/Theron/Include/ 
${SolutionDir}/Dependencies/Theron/Include/External/
)
add_subdirectory(NFComm/NFPluginLoader)
