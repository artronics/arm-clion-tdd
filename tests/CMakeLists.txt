project(tests)

set(CMAKE_CXX_STANDARD 11)

add_executable(
        unit_tests
        main.cpp
        example_add.cpp
)

target_link_libraries(
        unit_tests
        gtest
)

include_directories(
        ../vendor/gtest/googletest/include
        ../mocks
)