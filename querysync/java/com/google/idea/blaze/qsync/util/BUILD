package(default_visibility = [
    "//java/com/google/devtools/intellij/blaze/plugin/querysync:__subpackages__",
])

java_binary(
    name = "project_spec_builder",
    srcs = ["ProjectSpecBuilder.java"],
    main_class = "com.google.idea.blaze.qsync.util.ProjectSpecBuilder",
    visibility = ["//querysync:__pkg__"],
    deps = [
        ":cli_context",
        "//querysync/java/com/google/idea/blaze/qsync",
        "//querysync/java/com/google/idea/blaze/qsync/project",
        "//shared",
        "@com_google_guava_guava//jar",
        "@com_google_protobuf//:protobuf_java",
    ],
)

java_binary(
    name = "query_summarizer",
    srcs = ["QuerySummarizer.java"],
    main_class = "com.google.idea.blaze.qsync.util.QuerySummarizer",
    visibility = ["//querysync:__pkg__"],
    deps = [
        "//querysync/java/com/google/idea/blaze/qsync/project:snapshot_java_proto",
        "//querysync/java/com/google/idea/blaze/qsync/query",
    ],
)

java_library(
    name = "cli_context",
    srcs = ["CliContext.java"],
    deps = [
        "//shared",
    ],
)
