add_executable(lock lock.cpp)
target_compile_options(lock PUBLIC --std=c++20)

add_executable(lock_guard lock_guard.cpp)
target_compile_options(lock_guard PUBLIC --std=c++20)

add_executable(unique_lock unique_lock.cpp)
target_compile_options(unique_lock PUBLIC --std=c++20)