# 1. 최소 CMake 버전 및 프로젝트 정보 설정
cmake_minimum_required(VERSION 3.18)
project(ransomware-study LANGUAGES CXX)

# 2. C++ 표준 설정
set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

find_package(fmt REQUIRED)

# 3. 소스 파일로 실행 파일 만들기
add_executable(ransomware-study src/main.cpp)

target_link_libraries(ransomware-study PRIVATE
  fmt::fmt
)
