cmake_minimum_required(VERSION 3.10)
project(AmandsController)

# 查找 SFML 库
find_package(SFML 2.5 COMPONENTS graphics window system REQUIRED)

# 添加可执行文件
add_executable(AmandsController
    src/main.cpp  # 根据实际文件路径调整
)

# 链接 SFML 库
target_link_libraries(AmandsController
    sfml-graphics
    sfml-window
    sfml-system
)
