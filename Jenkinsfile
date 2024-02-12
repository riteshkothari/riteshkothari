standardPipeline {
    layer = "docitt"
    nuget_server = "http://nuget.ci/api/v2"
    nuget_targets = []
    skipFeatureBuilds = true
    docker_targets = [[
        name: "docitt-artifacts",
        dockerfile: "Dockerfile",
        repository: "docker.ci",
        image: "docitt-artifacts",
        chart: "docitt/docitt-artifacts"
    ]]
}