set(target "myassert")

add_executable(${target} src/main.c)

target_link_libraries(${target}
    libsel4
    libsel4assert
    libsel4startstop
)

AddRunTarget(${target})

add_dependencies(${target} sel4_kernel)
