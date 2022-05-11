cmake_minimum_required(VERSION 3.12)
project(cpp_app)

set(CMAKE_RUNTIME_OUTPUT_DIRECTORY "../bin")

include_directories(./include)
link_directories(./lib)

file(GLOB sourcefiles "src/*.h" "src/*.cpp")
add_executable(${PROJECT_NAME} ${sourcefiles}
)

