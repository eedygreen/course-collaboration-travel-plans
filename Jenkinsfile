pipeline {
  agent any
  stages {
    stage('permission') {
      agent {
        docker {
          image 'ubuntu'
          args '''sudo chown root:jenkins run/docker.soc
-p 3000:3000
'''
        }

      }
      steps {
        sh 'sudo chown root:jenkins run/docker.soc'
      }
    }

  }
}