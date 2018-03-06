pipeline {
  agent any
  stages {
    stage('Code') {
      parallel {
        stage('Clone code from git') {
          steps {
            echo 'Clone code'
          }
        }
        stage('SonarQube') {
          steps {
            echo 'Scan code via SOnarQube'
          }
        }
      }
    }
    stage('Build') {
      parallel {
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
      }
    }
    stage('Test') {
      steps {
        echo 'Test Feature via robot script'
      }
    }
    stage('Deploy') {
      steps {
        echo 'Deploy code to other ENV.'
      }
    }
  }
}