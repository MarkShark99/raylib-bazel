load("@rules_cc//cc:defs.bzl", "cc_binary")

cc_binary(
    name = "raylib-bazel",
    srcs = ["raylib-bazel.cpp"],
    linkopts = [
        "-framework CoreVideo",
        "-framework IOKit",
        "-framework Cocoa",
        "-framework GLUT",
        "-framework OpenGL",
    ],
    deps = [
        "@raylib",
    ],
)
