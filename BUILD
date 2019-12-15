load("@io_bazel_rules_docker//container:container.bzl", "container_push")

container_push(
    name = "push_server_image",
    format = "Docker",
    image = "//src/main/java/build/buildfarm:server.container",
    registry = "index.docker.io",
    repository = "softwaremotor/buildfarm-server",
    tag = "latest",
    visibility = ["//visibility:public"],
)

container_push(
    name = "push_worker_image",
    format = "Docker",
    image = "//src/main/java/build/buildfarm:buildfarm-operationqueue-worker.container",
    registry = "index.docker.io",
    repository = "softwaremotor/buildfarm-worker",
    tag = "latest",
    visibility = ["//visibility:public"],
)
