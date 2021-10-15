cmake_minimum_required(VERSION 3.20)
project(cuda_library CUDA)

set(CMAKE_CUDA_STANDARD 14)

add_library(cuda_library library.cu)

set_target_properties(cuda_library PROPERTIES
        CUDA_SEPARABLE_COMPILATION ON)
