pipeline {
  agent any
  stages {
    stage('Branch1') {
      parallel {
        stage('CommitCode To GIT') {
          steps {
            echo 'Commit code'
          }
        }
        stage('SonarQube') {
          steps {
            echo 'Scan code via SOnarQube'
          }
        }
        stage('Build APK') {
          steps {
            echo 'Build APK File'
          }
        }
        stage('Install APK') {
          steps {
            echo 'Install apk file to mobile'
          }
        }
        stage('Test') {
          steps {
            echo 'Test Feature via robot script'
          }
        }
      }
    }
    stage('Branch2') {
      steps {
        echo 'Prod ENV.'
      }
    }
  }
}