# ใน component/CMakeLists.txt
set(COMPONENT_SRCS
    "LED/src/led.c"    # แก้จาก LED.c เป็น led.c
)

set(COMPONENT_ADD_INCLUDEDIRS
    "LED/include"      # เพิ่ม /include
)

idf_component_register(
    SRCS ${COMPONENT_SRCS}
    INCLUDE_DIRS ${COMPONENT_ADD_INCLUDEDIRS}
)