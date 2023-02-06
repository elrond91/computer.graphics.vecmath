set(LIB_NAME vecmath)

set(CPP_FILES
    src/Matrix2f.cpp
    src/Matrix3f.cpp
    src/Matrix4f.cpp
    src/Quat4f.cpp
    src/Vector2f.cpp
    src/Vector3f.cpp
    src/Vector4f.cpp
    )

set(CPP_HEADER_DIR include)

set(CPP_HEADERS
    ${CPP_HEADER_DIR}/Matrix2f.h
    ${CPP_HEADER_DIR}/Matrix3f.h
    ${CPP_HEADER_DIR}/Matrix4f.h
    ${CPP_HEADER_DIR}/Quat4f.h
    ${CPP_HEADER_DIR}/Vector2f.h
    ${CPP_HEADER_DIR}/Vector3f.h
    ${CPP_HEADER_DIR}/Vector4f.h
    ${CPP_HEADER_DIR}/vecmath.h
    )

add_library(${LIB_NAME} STATIC ${CPP_FILES} ${CPP_HEADERS})
