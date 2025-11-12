if (CONFIG_MCUX_COMPONENT_middleware.cjson)
	mcux_component_version(1.7.19)
    mcux_add_source(
        SOURCES cJSON.h
                cJSON_Utils.h
                cJSON.c
                cJSON_Utils.c
    )
    mcux_add_include(
        INCLUDES ./
    )

    mcux_add_iar_configuration(
        CC "--diag_suppress=Pa084"
    )

    mcux_add_mdk_configuration(
        CC "-Wno-nan-infinity-disabled"
    )
endif()
