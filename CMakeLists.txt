# Minimum required CMake version
cmake_minimum_required(VERSION 3.10)

# Set project name and language (C)
project(Parser C)

# Set the C standard (optional but good practice)
set(CMAKE_C_STANDARD 11)

# Add the include directory for header files
include_directories(include)

# List of source files
set(SOURCES
    src/main.c
    src/utils.c
)

# Create an executable with the listed source files
add_executable(parser ${SOURCES})

# Optionally, add libraries or specific options if needed
# target_link_libraries(parser m)  # Uncomment if linking math library
