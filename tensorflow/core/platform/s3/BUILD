# Description:
# S3 support for TensorFlow.

package(default_visibility = ["//visibility:public"])

licenses(["notice"])  # Apache 2.0

exports_files(["LICENSE"])

load(
    "//tensorflow:tensorflow.bzl",
    "tf_cc_binary",
    "tf_cc_test",
)

cc_library(
    name = "aws_logging",
    srcs = [
        "aws_logging.cc",
    ],
    hdrs = [
        "aws_logging.h",
    ],
    deps = [
        "//tensorflow/core:lib",
        "//tensorflow/core:lib_internal",
        "//tensorflow/core/platform:stringprintf",
        "@aws",
    ],
    alwayslink = 1,
)
