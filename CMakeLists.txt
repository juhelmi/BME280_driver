set(BME280_SOURCES
    "bme280.c"
    )
set(BME280_HEADERS
    "bme280.h"
    "bme280_defs.h"
    )

add_library(${BME280_LIBRARY_NAME} STATIC
    ${BME280_SOURCES}
    ${BME280_HEADERS})

target_include_directories(${BME280_LIBRARY_NAME} PUBLIC
    "./")
