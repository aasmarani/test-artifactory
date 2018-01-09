pipeline {
  agent {
    node {
      label 'jdocker'
    }
    
  }
  stages {
    stage('fetch code') {
      steps {
        git(url: 'https://gitlabin.bajau.com/aasmarani/repo-multi-branch-pipeline.git', branch: 'master', credentialsId: 'gitlabincred')
      }
    }
    stage('build') {
      steps {
        echo 'build tools : npm & webpack'
      }
    }
  }
}