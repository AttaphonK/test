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
    stage('') {
      steps {
        mail(subject: 'testEmsil', body: 'Dear pae', cc: 'kidmaiaok_pae5.3@hotmail.com', to: 'attaphonkinnaree@gmail.com', from: 'attaphonkinnaree@gmail.com')
      }
    }
  }
}