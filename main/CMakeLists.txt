
add_executable(main main.cpp)

target_link_libraries(main PRIVATE Lib)

set(THREADS_PREFER_PTHREAD_FLAG ON)
find_package(Threads REQUIRED)

target_link_libraries(main 
                PRIVATE 
                      Threads::Threads
)

#target_compile_features(main PRIVATE cxx_std_17)


