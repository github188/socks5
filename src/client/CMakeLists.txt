PROJECT(Client CXX)

SET(HEAD_LIST
	../common/common.h)

SET(SRC_LIST
	main.c)

INCLUDE_DIRECTORIES(../common .)
LINK_DIRECTORIES(${CMAKE_BINARY_DIR}/lib)
ADD_EXECUTABLE(Client ${HEAD_LIST} ${SRC_LIST})
TARGET_LINK_LIBRARIES(Client libCommon.a)

