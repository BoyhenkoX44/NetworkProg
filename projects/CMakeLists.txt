list(APPEND COMMON_DEPENDENCIES common_utils common_net common_thread)

if (WIN32)
    LIST(APPEND COMMON_DEPENDENCIES wsock32 ws2_32)
elseif(LINUX)
    LIST(APPEND COMMON_DEPENDENCIES pthread)
endif()

add_subdirectory(Lab_1)
add_subdirectory(Lab_2)
add_subdirectory(Lab_3)
add_subdirectory(Lab_4)
add_subdirectory(Lab_5)
add_subdirectory(Pract_1)
add_subdirectory(Pract_3)
add_subdirectory(Pract_4)