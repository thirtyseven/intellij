package(default_visibility = [
    ":__subpackages__",
    "//base:__subpackages__",
    "//java/com/google/devtools/intellij/blaze/plugin/base:__subpackages__",
    "//java/com/google/devtools/intellij/blaze/plugin/querysync:__subpackages__",
    "//querysync/javatests:__subpackages__",
])

# A build rule to expose individual targets under java/ to users
java_library(
    name = "querysync",
    exports = [
        "//querysync/java/com/google/idea/blaze/qsync",
        "//querysync/java/com/google/idea/blaze/qsync/project",
        "//querysync/java/com/google/idea/blaze/qsync/project:project_java_proto",
        "//querysync/java/com/google/idea/blaze/qsync/query",
        "//querysync/java/com/google/idea/blaze/qsync/query:querysummary_java_proto",
    ],
)

test_suite(
    name = "querysync_tests",
    tests = [
        "//querysync/javatests/com/google/idea/blaze/qsync:AffectedPackagesTest",
        "//querysync/javatests/com/google/idea/blaze/qsync:GraphToProjectConverterTest",
        "//querysync/javatests/com/google/idea/blaze/qsync:PartialProjectRefreshTest",
        "//querysync/javatests/com/google/idea/blaze/qsync:ProjectRefresherTest",
        "//querysync/javatests/com/google/idea/blaze/qsync/project:BuildGraphTest",
        "//querysync/javatests/com/google/idea/blaze/qsync/project:SnapshotSerializationTest",
        "//querysync/javatests/com/google/idea/blaze/qsync/query:QuerySpecTest",
        "//querysync/javatests/com/google/idea/blaze/qsync/query:QuerySummaryTest",
    ],
)
