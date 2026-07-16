cmake_minimum_required(VERSION 3.20)

project(CppExpertScoringEngine)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_executable(
    cpp-expert-scoring-engine

    src/main.cpp

    src/app/Application.cpp

    src/api/ApiServer.cpp

    src/core/ScoringEngine.cpp
    src/core/Criterion.cpp
    src/core/Rule.cpp

    src/config/MethodologyLoader.cpp

    src/diagnostics/Logger.cpp
    src/diagnostics/Error.cpp
)

target_include_directories(
    cpp-expert-scoring-engine
    PRIVATE
    src
)