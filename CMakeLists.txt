cmake_minimum_required( VERSION 3.20 )

find_package( Basilisk CONFIG REQUIRED )

project( lib-basilisk Basilisk )

set(SOURCES
    "source/string.bslk"
)

source_group(TREE ${PROJECT_SOURCE_DIR} FILES ${SOURCES} ${HEADERS})

add_library( ${PROJECT_NAME} ${SOURCES} )