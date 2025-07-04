cmake_minimum_required(VERSION 3.10)
project(HandIsomorphism C)

add_library(handisomorphism STATIC
    hand_index.c
    deck.c
)

target_link_libraries(handisomorphism PRIVATE -lm)

target_include_directories(handisomorphism PUBLIC
    "${CMAKE_CURRENT_SOURCE_DIR}"
)