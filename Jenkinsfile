pipeline {
    agent {
      node {label 'App Connect Enterprise'}
    }
    environment {
    APPLICATION_NAME = 'App Connect Enterprise'
    GIT_REPO="https://github.com/ivancamargo190/IBM-AppConnectEnterprise-Openshift.git"
    GIT_BRANCH="dev"
    STAGE_TAG = "promoteToQA"
    DEV_PROJECT = "dev"
    STAGE_PROJECT = "stage"
    TEMPLATE_NAME = "App Connect Enterprise"
    ARTIFACT_FOLDER = "target"
    PORT = 8081;
}
stages {
    stage("Check SCM"){
    steps {
    git branch: "${GIT_BRANCH}", url: "${GIT_REPO}" // declared in environment
  }
    }
    stage("Build AppConnectEnterprise Image"){
    // Do Something
    }
    stage("Push to Registry"){
    // Do Something
    }
    stage("Deploy to RedHat Openshift"){
    // Do Something
    }
    stage("Check"){
    // Do Something
    }
}
}