cmake_minimum_required(VERSION 1.0.0)

find_library(LOG_LIBRARY log)

add_library(syscalls SHARED src/main/native/syscalls.c)
target_link_libraries(syscalls ${LOG_LIBRARY})
