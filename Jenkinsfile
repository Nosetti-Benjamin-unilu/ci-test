pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        withGradle() {
          build 'build'
        }

        mail(subject: 'builded', body: 'it vuilded', from: 'jenkins', to: 'benjamin.nosetti@gmail.com')
      }
    }

  }
}