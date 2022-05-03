#cmake 최소 버전 요구 사양
cmake_minimum_required(VERSION 3.8)

#프로젝트명 버전
project(myproject VERSION 1.0.0)

# 서브 디렉토리(src, library2)를 해당 폴더의 CMakefile을 실행
add_subdirectory(src)
add_subdirectory(library2)