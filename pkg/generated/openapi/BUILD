package(default_visibility = ["//visibility:public"])

licenses(["notice"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
)

go_library(
    name = "go_default_library",
    srcs = [
        "doc.go",
        "zz_generated.openapi.go",
    ],
    tags = ["automanaged"],
    deps = [
        "//pkg/api/resource:go_default_library",
        "//pkg/util/intstr:go_default_library",
        "//vendor:github.com/go-openapi/spec",
        "//vendor:k8s.io/apimachinery/pkg/genericapiserver/openapi/common",
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
