workspace(name = "opentelemetry")

load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

http_archive(
    name = "io_opentelemetry_cpp",
    sha256 = "4b6eeb852f075133c21b95948017f13a3e21740e55b921d27e42970a47314297",
    strip_prefix = "opentelemetry-cpp-1.20.0",
    urls = [
        "https://github.com/open-telemetry/opentelemetry-cpp/archive/refs/tags/v1.20.0.tar.gz",
    ],
)

# Load OpenTelemetry dependencies after the archive is downloaded
load("@io_opentelemetry_cpp//bazel:repository.bzl", "opentelemetry_cpp_deps")

opentelemetry_cpp_deps()
