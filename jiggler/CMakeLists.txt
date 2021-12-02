add_executable(jiggler
        jiggler.c
        usb_descriptors.c
        )

target_include_directories(jiggler PRIVATE ${CMAKE_CURRENT_LIST_DIR})

target_link_libraries(jiggler PRIVATE pico_stdlib tinyusb_device tinyusb_board pico_unique_id)
pico_add_extra_outputs(jiggler)

pico_set_program_url(jiggler https://github.com/argilo/pico-jiggler)
