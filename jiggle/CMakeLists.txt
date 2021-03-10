add_executable(jiggle
        jiggle.c
        usb_descriptors.c
        )

target_include_directories(jiggle PRIVATE ${CMAKE_CURRENT_LIST_DIR})

target_link_libraries(jiggle PRIVATE pico_stdlib tinyusb_device tinyusb_board)
pico_add_extra_outputs(jiggle)

# add url via pico_set_program_url
example_auto_set_url(jiggle)
