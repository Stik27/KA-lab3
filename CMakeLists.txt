project(lab3)

set(SOURCE_EXE main.cpp)
set(SOURCE_LIB hello.cpp factorial.cpp square.cpp)

add_library(foo STATIC ${SOURCE_LIB})
add_executable(main ${SOURCE_EXE})

target_link_libraries(main foo)
