ADD_EXECUTABLE(testcompression_wrapper testcompression_wrapper.c)
TARGET_LINK_LIBRARIES(testcompression_wrapper libcreaterepo_c ${GLIB2_LIBRARIES})
ADD_DEPENDENCIES(tests testcompression_wrapper)

ADD_EXECUTABLE(testload_metadata testload_metadata.c)
TARGET_LINK_LIBRARIES(testload_metadata libcreaterepo_c ${GLIB2_LIBRARIES})
ADD_DEPENDENCIES(tests testload_metadata)

ADD_EXECUTABLE(testmisc testmisc.c)
TARGET_LINK_LIBRARIES(testmisc libcreaterepo_c ${GLIB2_LIBRARIES})
ADD_DEPENDENCIES(tests testmisc)