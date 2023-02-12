workspace(name = "com_ethz_srl_nice2predict")

load("//tools/build_defs:externals.bzl", "new_patched_http_archive")
load("@bazel_tools//tools/build_defs/repo:git.bzl", "git_repository")
load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

http_archive(
    name = "org_pubref_rules_protobuf",
    sha256 = "fb9852446b5ba688cd7178a60ff451623e4112d015c6adfe0e9a06c5d2dedc08",
    strip_prefix = "rules_protobuf-0.8.1/",
    url = "https://github.com/pubref/rules_protobuf/archive/v0.8.1.tar.gz",
)

new_patched_http_archive(
    name = "com_github_sparsehash",
    build_file = "//third_party:BUILD.sparsehash",
    patch_file = "//third_party:sparsehash.patch",
    sha256 = "05e986a5c7327796dad742182b2d10805a8d4f511ad090da0490f146c1ff7a8c",
    strip_prefix = "sparsehash-sparsehash-2.0.3/",
    url = "https://github.com/sparsehash/sparsehash/archive/sparsehash-2.0.3.tar.gz",
)

git_repository(
    name = "com_google_googletest",
    remote = "https://github.com/google/googletest.git",
    tag = "release-1.11.0",
)

http_archive(
    name = "com_google_protobuf",
    sha256 = "51cec99f108b83422b7af1170afd7aeb2dd77d2bcbb7b6bad1f92509e9ccf8cb",
    strip_prefix = "protobuf-3.17.3",
    url = "https://github.com/protocolbuffers/protobuf/releases/download/v3.17.3/protobuf-cpp-3.17.3.tar.gz",
)

load("@com_google_protobuf//:protobuf_deps.bzl", "protobuf_deps")

protobuf_deps()

http_archive(
    name = "com_github_madler_zlib",
    build_file = "//third_party:BUILD.zlib",
    sha256 = "629380c90a77b964d896ed37163f5c3a34f6e6d897311f1df2a7016355c45eff",
    strip_prefix = "zlib-1.2.11",
    url = "https://github.com/madler/zlib/archive/refs/tags/v1.2.11.tar.gz",
)

http_archive(
    name = "com_github_grpc_grpc",
    sha256 = "f60e5b112913bf776a22c16a3053cc02cf55e60bf27a959fd54d7aaf8e2da6e8",
    strip_prefix = "grpc-1.38.1",
    url = "https://github.com/grpc/grpc/archive/refs/tags/v1.38.1.tar.gz",
)

load("@com_github_grpc_grpc//bazel:grpc_deps.bzl", "grpc_deps")

grpc_deps()

load("@com_github_grpc_grpc//bazel:grpc_extra_deps.bzl", "grpc_extra_deps")

grpc_extra_deps()

new_http_archive(
    name = "com_github_open_source_parsers_jsoncpp",
    build_file = "//third_party:BUILD.jsoncpp",
    sha256 = "3671ba6051e0f30849942cc66d1798fdf0362d089343a83f704c09ee7156604f",
    strip_prefix = "jsoncpp-1.8.3/",
    url = "https://github.com/open-source-parsers/jsoncpp/archive/1.8.3.tar.gz",
)

new_http_archive(
    name = "com_github_cinemast_libjson_rpc_cpp",
    build_file = "//third_party:BUILD.jsonrpc",
    sha256 = "888c10f4be145dfe99e007d5298c90764fb73b58effb2c6a3fc522a5b60a18c6",
    strip_prefix = "libjson-rpc-cpp-1.0.0",
    url = "https://github.com/cinemast/libjson-rpc-cpp/archive/v1.0.0.tar.gz",
)
