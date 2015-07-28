add_executable(myassert src/main.c)

target_link_libraries(myassert
    libsel4
    libsel4assert
    libsel4startstop
)

add_dependencies(myassert sel4_kernel)
