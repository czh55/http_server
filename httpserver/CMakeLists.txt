set(TARGET_NAME http_server)
#set(CMAKE_BUILD_TYPE Debug)

add_definitions(-std=c++11) # 这句是必须的，因为http_server中使用了C++的语法
add_executable(${TARGET_NAME} "http_server.cpp" "main.cpp" "mongoose.cpp")

target_link_libraries(${TARGET_NAME})
