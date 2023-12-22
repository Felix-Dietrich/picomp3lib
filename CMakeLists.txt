add_library(
    picomp3lib
	src/picomp3lib/mp3dec.h
	src/picomp3lib/mp3dec.c
    src/picomp3lib/mp3dec.c
    src/picomp3lib/bitstream.c
    src/picomp3lib/buffers.c
    src/picomp3lib/dct32.c
    src/picomp3lib/dequant.c
    src/picomp3lib/dqchan.c
    src/picomp3lib/huffman.c
    src/picomp3lib/hufftabs.c
    src/picomp3lib/imdct.c
    src/picomp3lib/mp3tabs.c
    src/picomp3lib/polyphase.c
    src/picomp3lib/scalfact.c
    src/picomp3lib/stproc.c
    src/picomp3lib/subband.c
    src/picomp3lib/trigtabs.c
)


target_include_directories(picomp3lib PUBLIC
"${CMAKE_CURRENT_SOURCE_DIR}/src")



target_link_libraries(picomp3lib PUBLIC
    pico_stdlib
)
