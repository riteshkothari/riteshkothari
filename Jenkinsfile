// node {

//   stage("pre-build check") {
//     String branch = env.BRANCH_NAME
//     String branchType 

//     echo 'Pulling... Branch : ' + branch

//     if(branch.contains('PR-')) {
//       branch = env.CHANGE_BRANCH
//       branchType = 'merge-request'
//     }
//     echo 'Pulling... Branch for merge request: ' + branch

//     if(branch == null) {
//       // print all environment variables
//       echo sh(returnStdout: true, script: 'env')
//     }
//   }
// }


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