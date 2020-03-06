set(ICON48
  fcitx-francais.png
)
set(ICON64
)

install(FILES
    ${ICON64}
    DESTINATION share/icons/hicolor/64x64/apps)

install(FILES
    ${ICON48}
    DESTINATION share/icons/hicolor/48x48/apps)

foreach(icon ${ICON48} ${ICON64})
    string(REPLACE "fcitx-" "" icon_new ${icon})
    install(FILES ${icon} RENAME ${icon_new} DESTINATION share/fcitx/imicon)
endforeach()
