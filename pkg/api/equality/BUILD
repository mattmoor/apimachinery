package(default_visibility = ["//visibility:public"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
)

go_library(
    name = "go_default_library",
    srcs = ["semantic.go"],
    importpath = "k8s.io/apimachinery/pkg/api/equality",
    deps = [
        "//pkg/api/resource:go_default_library",
        "//pkg/apis/meta/v1:go_default_library",
        "//pkg/conversion:go_default_library",
        "//pkg/fields:go_default_library",
        "//pkg/labels:go_default_library",
    ],
)

filegroup(
    name = "package-srcs",
    srcs = glob(["**"]),
    tags = ["automanaged"],
    visibility = ["//visibility:private"],
)

filegroup(
    name = "all-srcs",
    srcs = [":package-srcs"],
    tags = ["automanaged"],
)
