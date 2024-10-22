load("@com_google_protobuf_target//:protobuf.bzl", "py_proto_library")

licenses(["notice"])  # Apache 2.0

package(default_visibility = ["//visibility:public"])

py_proto_library(
    name = "config_py_pb2",
    srcs = [
        "config.proto",
    ],
    default_runtime = "@com_google_protobuf_target//:protobuf_python",
    protoc = "@com_google_protobuf_target//:protoc",
    deps = [
        "@com_google_protobuf_target//:protobuf_python",
    ],
)

py_proto_library(
    name = "metrics_for_slice_py_pb2",
    srcs = [
        "metrics_for_slice.proto",
    ],
    default_runtime = "@com_google_protobuf_target//:protobuf_python",
    protoc = "@com_google_protobuf_target//:protoc",
    deps = [
        "@com_google_protobuf_target//:protobuf_python",
    ],
)

py_proto_library(
    name = "validation_result_py_pb2",
    srcs = [
        "validation_result.proto",
    ],
    default_runtime = "@com_google_protobuf_target//:protobuf_python",
    protoc = "@com_google_protobuf_target//:protoc",
    deps = [
        ":config_py_pb2",
        ":metrics_for_slice_py_pb2",
        "@com_google_protobuf_target//:protobuf_python",
    ],
)

py_library(
    name = "all_protos",
    srcs = [],
    deps = [
        ":config_py_pb2",
        ":metrics_for_slice_py_pb2",
        ":validation_result_py_pb2",
    ],
)
