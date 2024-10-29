if (CONFIG_MCUX_COMPONENT_middleware.cjson)
    mcux_add_source(
        SOURCES cJSON.h
                cJSON_Utils.h
                cJSON.c
                cJSON_Utils.c
    )
    mcux_add_include(
        INCLUDES ./
    )
endif()
