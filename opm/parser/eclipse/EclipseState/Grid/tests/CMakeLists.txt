add_executable(runEclipseGridTests EclipseGridTests.cpp)
target_link_libraries(runEclipseGridTests Parser ${Boost_LIBRARIES})
add_test(NAME runEclipseGridTests WORKING_DIRECTORY ${PROJECT_SOURCE_DIR} COMMAND ${TEST_MEMCHECK_TOOL} ${EXECUTABLE_OUTPUT_PATH}/runEclipseGridTests )
