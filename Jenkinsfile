pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'npm --version'
        sh 'eval $(ssh-agent -s) && ssh-add ~/.ssh/id_rsa'
        sh 'npm install'
      }
    }
  }
}