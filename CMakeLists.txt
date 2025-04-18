cmake_minimum_required(VERSION 3.10)
project(HelloWorld)

add_executable(hello hello.cpp)

# Apply static linking flags only on Linux
if(CMAKE_SYSTEM_NAME STREQUAL "Linux")
    set_target_properties(hello PROPERTIES
        LINK_FLAGS "-static-libstdc++ -static-libgcc"
    )
endif()
