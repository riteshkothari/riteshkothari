node {

  stage("pre-build check") {
    String branch = env.BRANCH_NAME
    String branchType 

    echo 'Pulling... Branch : ' + branch

    if(branch.contains('PR-')) {
      branch = env.CHANGE_BRANCH
      branchType = 'merge-request'
    }
    echo 'Pulling... Branch for merge request: ' + branch

    if(branch == null) {
      // print all environment variables
      echo sh(returnStdout: true, script: 'env')
    }
  }
}
