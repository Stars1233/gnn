# Copybara rewrites load() statements back and forth; do not reformat.
# buildifier: disable=out-of-order-load, disable=same-origin-load
load("@tensorflow_gnn//tensorflow_gnn:tensorflow_gnn.bzl", "pytype_strict_library")

licenses(["notice"])

package(
    default_applicable_licenses = ["//tensorflow_gnn:license"],
    default_visibility = ["//visibility:public"],
)

pytype_strict_library(
    name = "test_utils",
    srcs = ["test_utils.py"],
)

pytype_strict_library(
    name = "api_utils",
    srcs = ["api_utils.py"],
)

pytype_strict_library(
    name = "tf_test_utils",
    srcs = ["tf_test_utils.py"],
    deps = [
        "//:expect_tensorflow_installed",
    ],
)
