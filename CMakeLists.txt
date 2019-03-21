cmake_minimum_required(VERSION 3.5)
project(ivcon)

find_package(ament_cmake REQUIRED)

add_executable(${PROJECT_NAME} src/ivcon.c)
target_link_libraries(${PROJECT_NAME} m)

install(TARGETS ${PROJECT_NAME}
  RUNTIME DESTINATION bin)

ament_package()
