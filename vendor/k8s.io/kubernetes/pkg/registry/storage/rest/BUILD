load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = ["storage_storage.go"],
    importpath = "k8s.io/kubernetes/pkg/registry/storage/rest",
    visibility = ["//visibility:public"],
    deps = [
        "//vendor/k8s.io/api/storage/v1:go_default_library",
        "//vendor/k8s.io/api/storage/v1alpha1:go_default_library",
        "//vendor/k8s.io/api/storage/v1beta1:go_default_library",
        "//vendor/k8s.io/apiserver/pkg/registry/generic:go_default_library",
        "//vendor/k8s.io/apiserver/pkg/registry/rest:go_default_library",
        "//vendor/k8s.io/apiserver/pkg/server:go_default_library",
        "//vendor/k8s.io/apiserver/pkg/server/storage:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/api/legacyscheme:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/apis/storage:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/registry/storage/storageclass/storage:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/registry/storage/volumeattachment/storage:go_default_library",
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
    visibility = ["//visibility:public"],
)
