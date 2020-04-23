pipeline {
  agent any
  stages {
    stage('permission') {
      agent {
        docker {
          image 'ubuntu'
          args '-p 3000:3000'
        }

      }
      steps {
        sh 'sudo chown root:jenkins run/docker.soc'
      }
    }

  }
}