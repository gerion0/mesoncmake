cmake_minimum_required(VERSION 3.10)
project(app VERSION 0.1 LANGUAGES C)

if (NOT SDK)
	message(FATAL_ERROR "This app needs the SDK. Specify SDK.")
endif ()

include_directories(${SDK}/include)
add_executable(app app.c ${SDK}/sdk.c)
