PROJECT(Laboratorium)

cmake_minimum_required(VERSION 2.4)

find_package(OpenIGTLink REQUIRED)

include(${OpenIGTLink_USE_FILE})

ADD_EXECUTABLE(NowyKlient  NowyKlient.cxx)
TARGET_LINK_LIBRARIES(NowyKlient OpenIGTLink)

ADD_EXECUTABLE(NowySerwer  NowySerwer.cxx)
TARGET_LINK_LIBRARIES(NowySerwer OpenIGTLink)
