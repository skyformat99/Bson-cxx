cmake_minimum_required (VERSION 3.2)
project (BSON)

set (CMAKE_CXX_STANDARD 11)

#FILES
set(SOURCE
	src/base64.cpp
  src/bson.cpp
  src/hex.cpp
  src/json.cpp
  src/parse_number.cpp
  src/time_support.cpp
  src/valid.cpp
)

include_directories(include)
set(INCLUDE
include/base64.h
include/bsonobjiterator.h
include/float_utils.h
include/status.h
include/base.h
include/bsontypes.h
include/hex.h
include/status_with.h
include/bsonelement.h
include/builder.h
include/json.h
include/string_data.h
include/bson-inl.h
include/cstdint.h
include/oid.h
include/string_data-inl.h
include/bsonobjbuilder.h
include/endian.h
include/ordering.h
include/time_support.h
include/bsonobj.h
include/errorcodes.h
include/parse_number.h
)

add_library(Template
    ${SOURCE}
    ${INCLUDE}
)
