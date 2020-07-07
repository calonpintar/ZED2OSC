project(ALL_BUILD)

################################################################################
# Source groups
################################################################################
set(ALL_FILES
)

################################################################################
# Target
################################################################################
add_executable(${PROJECT_NAME} ${ALL_FILES})

use_props(${PROJECT_NAME} "${CMAKE_CONFIGURATION_TYPES}" "${DEFAULT_CXX_PROPS}")
set_target_properties(${PROJECT_NAME} PROPERTIES
    VS_GLOBAL_KEYWORD "Win32Proj"
)
################################################################################
# Compile definitions
################################################################################
target_compile_definitions(${PROJECT_NAME} PRIVATE
    "_MBCS"
)

################################################################################
# Compile and link options
################################################################################
if(MSVC)
    target_compile_options(${PROJECT_NAME} PRIVATE
        ${DEFAULT_CXX_RUNTIME_LIBRARY};
        ${DEFAULT_CXX_DEBUG_INFORMATION_FORMAT};
        ${DEFAULT_CXX_EXCEPTION_HANDLING}
    )
    target_link_options(${PROJECT_NAME} PRIVATE
        /DEBUG:FULL
    )
endif()

################################################################################
# Dependencies
################################################################################
add_dependencies(${PROJECT_NAME}
    ZERO_CHECK
    OscDump
    OscReceiveTest
    OscSendTests
    OscUnitTests
    SimpleReceive
    SimpleSend
    ZED_Positional_Tracking
    oscpack
)

# Link with other targets.
target_link_libraries(${PROJECT_NAME} PUBLIC
    ZERO_CHECK
    OscDump
    OscReceiveTest
    OscSendTests
    OscUnitTests
    SimpleReceive
    SimpleSend
    ZED_Positional_Tracking
    oscpack
)



























project(ALL_BUILD)

################################################################################
# Source groups
################################################################################
set(ALL_FILES
)

################################################################################
# Target
################################################################################
add_executable(${PROJECT_NAME} ${ALL_FILES})

use_props(${PROJECT_NAME} "${CMAKE_CONFIGURATION_TYPES}" "${DEFAULT_CXX_PROPS}")
set_target_properties(${PROJECT_NAME} PROPERTIES
    VS_GLOBAL_KEYWORD "Win32Proj"
)
################################################################################
# Compile definitions
################################################################################
target_compile_definitions(${PROJECT_NAME} PRIVATE
    "_MBCS"
)

################################################################################
# Compile and link options
################################################################################
if(MSVC)
    target_compile_options(${PROJECT_NAME} PRIVATE
        ${DEFAULT_CXX_RUNTIME_LIBRARY};
        ${DEFAULT_CXX_DEBUG_INFORMATION_FORMAT};
        ${DEFAULT_CXX_EXCEPTION_HANDLING}
    )
    target_link_options(${PROJECT_NAME} PRIVATE
        /DEBUG:FULL
    )
endif()

################################################################################
# Dependencies
################################################################################
add_dependencies(${PROJECT_NAME}
    ZERO_CHECK
    OscDump
    OscReceiveTest
    OscSendTests
    OscUnitTests
    SimpleReceive
    SimpleSend
    ZED_Positional_Tracking
    oscpack
)

# Link with other targets.
target_link_libraries(${PROJECT_NAME} PUBLIC
    ZERO_CHECK
    OscDump
    OscReceiveTest
    OscSendTests
    OscUnitTests
    SimpleReceive
    SimpleSend
    ZED_Positional_Tracking
    oscpack
)



























project(ALL_BUILD)

################################################################################
# Source groups
################################################################################
set(ALL_FILES
)

################################################################################
# Target
################################################################################
add_executable(${PROJECT_NAME} ${ALL_FILES})

use_props(${PROJECT_NAME} "${CMAKE_CONFIGURATION_TYPES}" "${DEFAULT_CXX_PROPS}")
set_target_properties(${PROJECT_NAME} PROPERTIES
    VS_GLOBAL_KEYWORD "Win32Proj"
)
################################################################################
# Compile definitions
################################################################################
target_compile_definitions(${PROJECT_NAME} PRIVATE
    "_MBCS"
)

################################################################################
# Compile and link options
################################################################################
if(MSVC)
    target_compile_options(${PROJECT_NAME} PRIVATE
        ${DEFAULT_CXX_RUNTIME_LIBRARY};
        ${DEFAULT_CXX_DEBUG_INFORMATION_FORMAT};
        ${DEFAULT_CXX_EXCEPTION_HANDLING}
    )
    target_link_options(${PROJECT_NAME} PRIVATE
        /DEBUG:FULL
    )
endif()

################################################################################
# Dependencies
################################################################################
add_dependencies(${PROJECT_NAME}
    ZERO_CHECK
    OscDump
    OscReceiveTest
    OscSendTests
    OscUnitTests
    SimpleReceive
    SimpleSend
    ZED_Positional_Tracking
    oscpack
)

# Link with other targets.
target_link_libraries(${PROJECT_NAME} PUBLIC
    ZERO_CHECK
    OscDump
    OscReceiveTest
    OscSendTests
    OscUnitTests
    SimpleReceive
    SimpleSend
    ZED_Positional_Tracking
    oscpack
)

