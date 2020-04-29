pipeline {
  agent any
  stages {

    stage('build') {
      steps {
        buildName "${JOB_NAME}"
        build job: ${buildName}, propagate: false
        echo 'Build success'
      }
    }
  }
}
