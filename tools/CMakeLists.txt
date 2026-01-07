add_library(EditorApp STATIC
    editor/src/EditorApp.cpp
)

target_include_directories(EditorApp PUBLIC
    ${CMAKE_CURRENT_SOURCE_DIR}/include
)

#target_link_libraries(EditorApp PUBLIC
#        # Framework
#        # EngineCore
#        # SystemUI
#)

add_library(Apps::EditorApp ALIAS EditorApp)
