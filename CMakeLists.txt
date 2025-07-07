cmake_minimum_required(VERSION 3.10)
project(solo_axis_igh C)

# 编译选项
set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -Wall -O3 -g")

# 源文件（匹配所有 .c 文件）
file(GLOB SRC_FILES *.c)

# 添加可执行文件
add_executable(solo_axis_igh ${SRC_FILES})

# 链接库
target_link_libraries(solo_axis_igh
        m
        ethercat
        rt
        pthread
)
