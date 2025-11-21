cmake_minimum_required(VERSION 3.5)
project(myrobot)

# Use ament_cmake build system
find_package(ament_cmake REQUIRED)

# Install folders (if they exist)
install(
  DIRECTORY
    meshes
    urdf
  DESTINATION
    share/${PROJECT_NAME}
)

ament_package()