cmake_minimum_required(VERSION 3.0.0)
project(tahir VERSION 0.1.0)
set(CMAKE_CXX_STANDARD 17)

set(CMAKE_GENERATOR "Unix Makefiles")
message("Merhaba Dostum ${CMAKE_GENERATOR}")



file(GLOB ATI_SRC CONFIGURE_DEPENDS ${PROJECT_SOURCE_DIR}/src/*.cpp ${PROJECT_SOURCE_DIR}/lib/*.h)
message("ATI SRC ${ATI_SRC}")

add_executable(tahir ${ATI_SRC})

