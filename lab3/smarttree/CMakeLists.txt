
project(smarttree)

set(HEDEAR_FILES SmartTree.h)
set(SOURCE_FILES SmartTree.cpp)

add_library(libsmarttree STATIC ${SOURCE_FILES})
target_include_directories(libsmarttree PUBLIC .)

add_executable(smarttree ${SOURCE_FILES} main.cpp)

target_link_libraries(smarttree libsmarttree)
