include_directories(${PROJECT_SOURCE_DIR}/../include)

aux_source_directory(${PROJECT_SOURCE_DIR}/src SRC_FILES)

add_library(uvkafka_a STATIC ${SRC_FILES})

add_library(uvkafka SHARED ${SRC_FILES})

target_link_libraries(uvkafka uv_a)