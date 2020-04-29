pipeline {
  agent any
  stages {

    stage('build') {
      steps {
        build job: 'SampleAppCICD', propagate: false
        echo 'Build success'
      }
    }
  }
}
