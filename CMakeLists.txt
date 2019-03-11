cmake_minimum_required(VERSION 3.13)

add_subdirectory(libs/libpancake)

#find_package(pancake REQUIRED)
add_executable(mellow src/main.cpp)

target_include_directories(mellow PRIVATE pancake)
target_link_libraries(mellow pancake)
