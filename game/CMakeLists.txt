add_library(GameApp STATIC
    src/GameApp.cpp
)

target_include_directories(GameApp PUBLIC
    ${CMAKE_CURRENT_SOURCE_DIR}/include
)

# 依存（必要なものだけ残す）
#target_link_libraries(GameApp PUBLIC
#        # Framework
#        # EngineCore
#        # SystemInput
#        # SystemUI
#)

# link を読みやすくするための alias（任意だがオススメ）
add_library(Apps::GameApp ALIAS GameApp)
