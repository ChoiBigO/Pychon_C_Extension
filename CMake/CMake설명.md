# CMake

## CMake 사용 이유
- CMake는 Makefile을 만들어 주는 툴이다.
- Makefile : 빌드를 편리하게 해주는 일종의 빌드 스크립트 이다.
- Makefile을 사용하는 이유는 Incremental build 방식을 사용하기 떄문이다.
- Incremental build : 처음에는 전체를 빌드 하고, 이후에 수정된 파일에 대해서는 그 소스파일에 연관된 것만 빌드하여 시간을 줄여주는 빌드 방식이다.
- CMake는 여러개의 플랫폼에 맞는 템플릿을 생성해 주기 때문에 다양한 플랫폼에서 빌드가 가능하다.

## 실습
- ./example 에 CMake 간단 예제
- build dir(build된 파일들이 존재할 폴더) 생성
- cd build => ``` cmake ..```