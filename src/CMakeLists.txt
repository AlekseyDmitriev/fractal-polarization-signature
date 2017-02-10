cmake_minimum_required(VERSION 2.8)

set(NAME FPS)

project(${NAME})

set(SOURCES FractalPolarizationSignature.cxx 
	SignaturesCalculationHelper.cxx
	)
include_directories (${PROJECT_SOURCE_DIR})

add_executable(FractalPolarizationSignature  ${SOURCES})
target_link_libraries(FractalPolarizationSignature ${OTB_LIBRARIES}) 



