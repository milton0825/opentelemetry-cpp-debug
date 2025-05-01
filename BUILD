licenses(["notice"])  # Apache 2

cc_binary(
    name = "otel_test",
    srcs = ["main.cc"],
    copts = ["-std=c++17"],
    linkopts = ["-std=c++17"],
    deps = [
        "@io_opentelemetry_cpp//api",
        "@io_opentelemetry_cpp//exporters/ostream:ostream_span_exporter",
        "@io_opentelemetry_cpp//exporters/otlp:otlp_http_exporter",
    ],
)
