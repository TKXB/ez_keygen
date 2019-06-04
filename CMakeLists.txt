cmake_minimum_required(VERSION 3.7)
project(ezviz_keygen)

set(CMAKE_C_STANDARD 99)

add_executable(ecc_key_gen ecc_key_gen.c util.h util.c)
target_link_libraries(ecc_key_gen mbedcrypto)
