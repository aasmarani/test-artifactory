pipeline {
  agent {
    node {
      label 'jslave'
    }
    
  }
  stages {
    stage('fetch code') {
      steps {
        git(url: 'https://github.com/aasmarani/react-example.git', branch: 'master', credentialsId: 'github-cred')
      }
    }
  }
}