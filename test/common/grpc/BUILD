licenses(["notice"])  # Apache 2

load(
    "//bazel:envoy_build_system.bzl",
    "envoy_cc_test",
    "envoy_package",
)

envoy_package()

envoy_cc_test(
    name = "codec_test",
    srcs = ["codec_test.cc"],
    deps = [
        "//source/common/buffer:buffer_lib",
        "//source/common/grpc:codec_lib",
        "//test/proto:helloworld_proto",
    ],
)

envoy_cc_test(
    name = "common_test",
    srcs = ["common_test.cc"],
    deps = [
        "//source/common/grpc:common_lib",
        "//source/common/http:headers_lib",
        "//test/mocks/upstream:upstream_mocks",
        "//test/proto:helloworld_proto",
    ],
)

envoy_cc_test(
    name = "http1_bridge_filter_test",
    srcs = ["http1_bridge_filter_test.cc"],
    deps = [
        "//source/common/buffer:buffer_lib",
        "//source/common/grpc:http1_bridge_filter_lib",
        "//source/common/http:header_map_lib",
        "//test/mocks/http:http_mocks",
        "//test/mocks/upstream:upstream_mocks",
        "//test/test_common:utility_lib",
    ],
)

envoy_cc_test(
    name = "grpc_web_filter_test",
    srcs = ["grpc_web_filter_test.cc"],
    deps = [
        "//source/common/grpc:grpc_web_filter_lib",
        "//test/mocks/http:http_mocks",
        "//test/mocks/upstream:upstream_mocks",
        "//test/test_common:utility_lib",
    ],
)

envoy_cc_test(
    name = "rpc_channel_impl_test",
    srcs = ["rpc_channel_impl_test.cc"],
    deps = [
        "//source/common/grpc:common_lib",
        "//source/common/grpc:rpc_channel_lib",
        "//source/common/http:message_lib",
        "//test/mocks/grpc:grpc_mocks",
        "//test/mocks/upstream:upstream_mocks",
        "//test/proto:helloworld_proto",
        "//test/test_common:utility_lib",
    ],
)
