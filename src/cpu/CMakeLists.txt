add_executable(add-cpu)

target_sources(add-cpu PRIVATE add.cpp)

set_target_properties(add-cpu   PROPERTIES
                                CXX_STANDARD 17)
