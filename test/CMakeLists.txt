# find GTest
find_package(GTest REQUIRED)
include_directories(${GTEST_INCLUDE_DIRS})

# include src files
include_directories(${stats_SOURCE_DIR}/src)

# include test files
add_executable(tests
    tests.cpp
)

target_link_libraries(tests ${GTEST_LIBRARIES} pthread statslib)