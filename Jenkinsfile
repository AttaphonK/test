pipeline {
  agent any
  stages {
    stage('StepOne') {
      steps {
        echo 'Let start'
      }
    }
    stage('Checkout from GIT') {
      steps {
        git(url: 'https://gitlab.com/aware-automate/myChannelDevOPS.git', branch: 'mastere')
      }
    }
    stage('stop') {
      steps {
        echo 'Stop JA'
      }
    }
  }
}