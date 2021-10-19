cmake_minimun_required (Version 3.8)

#if (${CMAKE_VERSION} VERSION_LESS 3.12)
 #   cmake_policy(VERSION ${CMAKE_VERSION})
#endif()

project ("beispiel")

#Add the cmake folder so the FindSphinx module is found
set(CMAKE_MODULE_PATH "${PROJECT_SOURCE_DIR}/cmake" ${CMAKE_MODULE_PATH})

add_subdirectory ("src")
add_subdirectory ("docs")
