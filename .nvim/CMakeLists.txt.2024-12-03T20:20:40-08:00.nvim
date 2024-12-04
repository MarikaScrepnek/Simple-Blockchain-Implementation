cmake_minimum_required(VERSION 3.14)

project("A12 Marika Screpnek." LANGUAGES C CXX)

set(CMAKE_C_STANDARD 99)
set(CMAKE_C_STANDARD_REQUIRED ON)
set(CMAKE_C_EXTENSIONS OFF)
set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -fsanitize=address")

find_package(OpenSSL REQUIRED)

file(GLOB BLOCKCHAIN_SOURCES "src/*.c")

add_executable(blockchain ${BLOCKCHAIN_SOURCES})

include_directories(include)

target_link_libraries(blockchain PRIVATE OpenSSL::Crypto OpenSSL::SSL
  "${CMAKE_SOURCE_DIR}/lib/libcheck-x86_64.so")

set(CMAKE_EXPORT_COMPILE_COMMANDS_ON)

target_compile_options(blockchain PRIVATE ${SANITIZER_FLAGS})
target_link_libraries(blockchain PRIVATE ${SANITIZER_FLAGS})
