cmake_minimum_required(VERSION 3.13)

# case libs/libpancake
add_subdirectory(libs/libpancake)
add_executable(mellow src/main.cpp)
target_include_directories(mellow PRIVATE pancake)
target_link_libraries(mellow pancake)

# case make install
# find_package(pancake REQUIRED)
# add_executable(mellow src/main.cpp)
# target_include_directories(mellow PRIVATE pancake::pancake)
# target_link_libraries(mellow pancake::pancake)
