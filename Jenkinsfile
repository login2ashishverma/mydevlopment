pipeline {
  agent any
  stages {

    stage('build') {
      steps {
        build job: "${JOB_NAME}", propagate: false
        echo 'Build success'
      }
    }
  }
}
