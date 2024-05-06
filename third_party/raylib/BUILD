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
    lib_source = "@raylib//:all_srcs",
    linkopts = [
        "-framework CoreVideo",
        "-framework IOKit",
        "-framework Cocoa",
        "-framework GLUT",
        "-framework OpenGL",
    ],
    out_static_libs = ["libraylib.a"],
)
