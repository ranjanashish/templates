cmake_minimum_required(VERSION 2.8)

# FindBoost.cmake
#################
set(Boost_USE_STATIC_LIBS OFF) 
set(Boost_USE_MULTITHREADED ON) 
set(Boost_USE_STATIC_RUNTIME OFF) 
find_package(Boost COMPONENTS filesystem REQUIRED)
if(Boost_FOUND)
    include_directories(${Boost_INCLUDE_DIRS})
    add_executable(progname file1.cpp file2.cpp)
    target_link_libraries(progname ${Boost_LIBRARIES})
endif()

# FindCUDA.cmake
################

# FindCurses.cmake
##################
set(CURSES_NEED_NCURSES TRUE) 
find_package(Curses REQUIRED)

# FindGnuplot.cmake
###################

# FindMPI.cmake
###############

# FindOpenGL.cmake
##################

# FindOpenMP.cmake
##################

# OpenCVConfig.cmake
####################

