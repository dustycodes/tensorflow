package(default_visibility = ["//tensorflow:internal"])

load("@io_bazel_rules_closure//closure:defs.bzl", "web_library")

licenses(["notice"])  # Apache 2.0

# bazel run //third_party/tensorflow/tensorboard/components/tf_distribution_dashboard/demo
web_library(
    name = "demo",
    srcs = ["index.html"],
    path = "/tf-distribution-dashboard/demo",
    deps = [
        "//tensorflow/tensorboard/components/tf_distribution_dashboard",
        "//tensorflow/tensorboard/components/tf_distribution_dashboard/demo/data",
        "//tensorflow/tensorboard/components/tf_imports:d3",
        "@org_polymer_iron_demo_helpers",
        "@org_polymer_paper_styles",
        "@org_polymer_webcomponentsjs",
    ],
)

filegroup(
    name = "all_files",
    srcs = glob(["**"]),
    tags = ["notsan"],
)
