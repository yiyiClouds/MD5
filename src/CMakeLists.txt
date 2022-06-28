add_library(md5_static STATIC md5.cpp)
set_target_properties(md5_static PROPERTIES OUTPUT_NAME "md5")

install (TARGETS md5_static
  RUNTIME DESTINATION bin
  LIBRARY DESTINATION lib
  ARCHIVE DESTINATION lib)

install (FILES md5.h DESTINATION "include")