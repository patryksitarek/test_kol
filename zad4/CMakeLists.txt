cmake_minimum_required(VERSION 3.13.4)
project(StudentTest)

include_directories(include)


set(PROJECT_LINK_LIBS testStudent.a) #.dylib for shared

link_directories("~/laborki_git/kolokwium/zad4/lib/")

add_executable(myProgram "src/libtest.cpp")

install(TARGETS myProgram DESTINATION "~/laborki_git/kolokwium/zad4/bin/")

target_link_libraries(myProgram ${PROJECT_LINK_LIBS} )
