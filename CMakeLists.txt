cmake_minimum_required(VERSION 3.22)
project(untitled)

set(CMAKE_CXX_STANDARD 14)

include_directories(./wkhtmltopdf/include)

link_libraries(wkhtmltox)

add_executable(SimpleLatexRender main.cpp)

target_link_directories(SimpleLatexRender PRIVATE ./wkhtmltopdf/bin)
