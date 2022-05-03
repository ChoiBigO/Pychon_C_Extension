#라이브러리를 추가한다.
add_library(
    hello
    hello.hpp
    hello.cpp
)

#main.cpp의 파일을 가주고 main이라는 바이너리를 생성한다.
add_executable(main main.cpp)

#라이브러리 링킹
target_link_libraries(main PRIVATE hello)
target_link_libraries(main PRIVATE library2)    # 해당 타켓(library2)에 맞는 link를 해주고 library2에 속한 include 값을 자동으로 프로젝트에 넣어준다.