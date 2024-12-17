package(
    default_visibility = ["//visibility:public"],
)

cc_library(
    name = "spirv-cross-core",
    srcs = [
        "spirv_cfg.cpp",
        "spirv_cross.cpp",
        "spirv_cross_parsed_ir.cpp",
        "spirv_parser.cpp",
    ],
    hdrs = [
        "GLSL.std.450.h",
        "spirv.hpp",
        "spirv_cfg.hpp",
        "spirv_common.hpp",
        "spirv_cross.hpp",
        "spirv_cross_containers.hpp",
        "spirv_cross_error_handling.hpp",
        "spirv_cross_parsed_ir.hpp",
        "spirv_parser.hpp",
    ],
)

cc_library(
    name = "spirv-cross-c",
    srcs = [
        "spirv_cross_c.cpp",
    ],
    hdrs = [
        "spirv.h",
        "spirv_cross_c.h",
    ],
    deps = [
        ":spirv-cross-core",
    ],
)

cc_library(
    name = "spirv-cross-glsl",
    srcs = [
        "spirv_glsl.cpp",
    ],
    hdrs = [
        "spirv_glsl.hpp",
    ],
    deps = [
        ":spirv-cross-core",
    ],
)

cc_library(
    name = "spirv-cross-cpp",
    srcs = [
        "spirv_cpp.cpp",
    ],
    hdrs = [
        "spirv_cpp.hpp",
    ],
    deps = [
        ":spirv-cross-glsl",
    ],
)

cc_library(
    name = "spirv-cross-msl",
    srcs = [
        "spirv_msl.cpp",
    ],
    hdrs = [
        "spirv_msl.hpp",
    ],
    deps = [
        ":spirv-cross-glsl",
    ],
)

cc_library(
    name = "spirv-cross-hlsl",
    srcs = [
        "spirv_hlsl.cpp",
    ],
    hdrs = [
        "spirv_hlsl.hpp",
    ],
    deps = [
        ":spirv-cross-glsl",
    ],
)

cc_library(
    name = "spirv-cross-reflect",
    srcs = [
        "spirv_reflect.cpp",
    ],
    hdrs = [
        "spirv_reflect.hpp",
    ],
    deps = [
        ":spirv-cross-glsl",
    ],
)

cc_library(
    name = "spirv-cross-util",
    srcs = [
        "spirv_cross_util.cpp",
    ],
    hdrs = [
        "spirv_cross_util.hpp",
    ],
    deps = [
        ":spirv-cross-core",
    ],
)
