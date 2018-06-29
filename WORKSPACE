load(
    "@bazel_tools//tools/build_defs/repo:git.bzl",
    system_git_repository = "git_repository",
)

system_git_repository(
    name = "bazel_skylib",
    remote = "https://github.com/bazelbuild/bazel-skylib.git",
    commit = "ff23a62c57d2912c3073a69c12f42c3d6e58a957",
    verbose = True,
)

system_git_repository(
    name = "io_bazel_rules_go",
    remote = "https://github.com/bazelbuild/rules_go.git",
    commit = "d850f8bbd15d94ce11a078b3933e92ebbf09f715",
    verbose = True,
)

system_git_repository(
    name = "bazel_gazelle",
    remote = "https://github.com/bazelbuild/bazel-gazelle.git",
    commit = "394f5355e0b91940f45bba9a705fb4382b234316",
    verbose = True,
)

load("@io_bazel_rules_go//go:def.bzl", "go_rules_dependencies", "go_register_toolchains")

go_rules_dependencies()

go_register_toolchains()

load("@bazel_gazelle//:deps.bzl", "gazelle_dependencies")

gazelle_dependencies()
