load("@rules_foreign_cc//foreign_cc:defs.bzl", "cmake")

package(
    default_visibility = ["//visibility:public"],
)

filegroup(
    name = "all_srcs",
    srcs = glob(["**"]),
)

cmake(
    name = "raylib",
    cache_entries = {
        "CMAKE_APPLE_SILICON_PROCESSOR": "arm64",
        "CMAKE_OSX_ARCHITECTURES": "arm64",
    },
    lib_source = "@raylib//:all_srcs",
    out_static_libs = ["libraylib.a"],
)
