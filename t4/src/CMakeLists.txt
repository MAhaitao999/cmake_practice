CMAKE_MINIMUM_REQUIRED(VERSION 3.5)
FIND_PATH(myHeader hello.h)
IF(myHeader)
    INCLUDE_DIRECTORIES(${myHeader})
ENDIF(myHeader)
# INCLUDE_DIRECTORIES(/usr/include/hello)
ADD_EXECUTABLE(main main.c)
# TARGET_LINK_LIBRARIES(main hello) # 必须放在ADD_EXECUTABLE(main main.c)后面
TARGET_LINK_LIBRARIES(main libhello.a) # 必须放在ADD_EXECUTABLE(main main.c)后面
