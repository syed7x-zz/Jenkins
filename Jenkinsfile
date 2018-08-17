pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'npm --version'
        sh 'eval $(ssh-agent -s) && yes y |ssh-keygen -q -t rsa -N \'\' &&ssh-add ~/.ssh/id_rsa'
        sh 'npm --install'
      }
    }
  }
}