#라이브러리를 추가한다.
add_library(
    library2 
    library2.cpp
    library2.hpp
)

# 종속된 프로젝트를 include 해줄 수 있는 키워드 이다.
# library2 라이브러리를 사용하게 된 경우 해당 소스코드를 include 해주는 역할을 한다.
# visual studio에서 c/c++ > 일반 > 추가포함 디렉터리에 해당 경로가 추가 된다.
# 이를 통해 library2.hpp를 main에서 include 할수 있게 된다.
target_include_directories(library2 PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})