CMAKE_MINIMUM_REQUIRED(VERSION 3.10)

PROJECT(LX-RDMA-RPC)

set(CMAKE_CXX_STANDARD 11)


# 添加gtest的源码目录
add_subdirectory(/usr/src/gtest ${CMAKE_BINARY_DIR}/gtest)

# 包括gtest的头文件
include_directories(${gtest_SOURCE_DIR}/include ${gtest_SOURCE_DIR})
# find_package(Boost 1.53.0 REQUIRED COMPONENTS system thread)

# if(Boost_FOUND)
#     include_directories(${Boost_INCLUDE_DIRS})
# endif()

# find_package(PkgConfig REQUIRED)
# pkg_check_modules(PCRECPP REQUIRED libpcrecpp)
# include_directories(${PCRECPP_INCLUDE_DIRS})

include_directories(obj.240428/build-ubuntu1804)

add_definitions(-DTESTING=1)


# target_link_libraries(server profiler ibverbs ${PCRECPP_LIBRARIES} Boost::system Boost::thread )


add_executable(TcpTransportTest src/TcpTransportTest.cc)

target_link_libraries(TcpTransportTest gtest gtest_main)