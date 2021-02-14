add_library(statslib stats.h stats.cpp)

target_include_directories(statslib PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})

#target_sources(
#    statslib
#    PRIVATE
#        stats.h
#    PUBLIC
#        ${CMAKE_CURRENT_LIST_DIR}/stats.h
#)

add_executable(stats main.cpp)

target_link_libraries(stats LINK_PUBLIC statslib)