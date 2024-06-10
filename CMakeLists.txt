# Copyright (c) 2020 The ZMK Contributors
# SPDX-License-Identifier: MIT

target_sources_ifdef(CONFIG_ZMK_DISPLAY app PRIVATE src/display/main.c)
target_sources_ifdef(CONFIG_ZMK_DISPLAY_STATUS_SCREEN_BUILT_IN app PRIVATE src/display/status_screen.c)

add_subdirectory_ifdef(CONFIG_ZMK_DISPLAY src/display/widgets/)
