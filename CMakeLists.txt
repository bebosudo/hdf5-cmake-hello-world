project(myproj LANGUAGES C)

find_package(HDF5 REQUIRED COMPONENTS C HL)

add_executable(myprog myprog.c)
target_link_libraries(myprog PRIVATE HDF5::HDF5)
