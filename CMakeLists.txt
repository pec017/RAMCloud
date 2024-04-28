CMAKE_MINIMUM_REQUIRED(VERSION 3.10)

PROJECT(LX-RDMA-RPC)

set(CMAKE_CXX_STANDARD 11)

# find_package(Boost 1.53.0 REQUIRED COMPONENTS system thread)

# if(Boost_FOUND)
#     include_directories(${Boost_INCLUDE_DIRS})
# endif()

# find_package(PkgConfig REQUIRED)
# pkg_check_modules(PCRECPP REQUIRED libpcrecpp)
# include_directories(${PCRECPP_INCLUDE_DIRS})

# add_executable(server src/server.cc
#         src/InfRcTransport.cc
#         src/TcpTransport.cc
#         src/Buffer.cc
#         src/ServiceLocator.cc
#         src/Logging.cc
#         # src/TestUtil.cc # My gtest is newest, which needs C++14. To enable gperftools, you need to use C++11
#         src/TransportManager.cc
#         src/Common.cc
#         src/IpAddress.cc
#         src/Transport.cc
#         src/Infiniband.cc
#         src/Metrics.cc
#         src/BenchUtil.cc
#         src/Dispatch.cc
#         src/TimeCounter.cc
#         src/ServiceManager.cc
#         src/Status.cc)

# target_link_libraries(server profiler ibverbs ${PCRECPP_LIBRARIES} Boost::system Boost::thread )

# add_executable(client src/client.cc
#         src/InfRcTransport.cc
#         src/TcpTransport.cc
#         src/Buffer.cc
#         src/ServiceLocator.cc
#         src/Logging.cc
#         # src/TestUtil.cc # My gtest is newest, which needs C++14. To enable gperftools, you need to use C++11
#         src/TransportManager.cc
#         src/Common.cc
#         src/IpAddress.cc
#         src/Transport.cc
#         src/Infiniband.cc
#         src/Metrics.cc
#         src/BenchUtil.cc
#         src/Dispatch.cc
#         src/TimeCounter.cc
#         src/ServiceManager.cc
#         src/Status.cc)

# target_link_libraries(client profiler ibverbs ${PCRECPP_LIBRARIES} Boost::system Boost::thread)


# add_executable(infRcTest src/InfRcTransportTest.cc
#         src/TestUtil.cc
#         src/InfRcTransport.cc
#         src/TcpTransport.cc
#         src/Buffer.cc
#         src/ServiceLocator.cc
#         src/Logging.cc
#         src/TestUtil.cc
#         src/TransportManager.cc
#         src/Common.cc
#         src/IpAddress.cc
#         src/Transport.cc
#         src/Infiniband.cc
#         src/Metrics.cc
#         src/BenchUtil.cc
#         src/Dispatch.cc
#         src/TimeCounter.cc
#         src/ServiceManager.cc
#         src/Status.cc)
# # set C++14 to use gtest on my system, you can remove this property to use an old version of gtest
# set_target_properties(infRcTest PROPERTIES
# CXX_STANDARD 14
# CXX_STANDARD_REQUIRED YES
# CXX_EXTENSIONS NO
# )

# target_link_libraries(infRcTest ibverbs ${PCRECPP_LIBRARIES} gtest Boost::system Boost::thread)

