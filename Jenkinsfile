pipeline {
  agent {
    docker {
      image 'node:6-alpine'
      args '-p 3000:3000'
    }

  }
  stages {
    stage('Build') {
      steps {
        sh 'sudo npm install --unsafe-perm=true --allow-root --registry=https://registry.npm.taobao.org'
      }
    }

  }
}