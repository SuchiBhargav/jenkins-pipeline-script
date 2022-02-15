pipeline {
  agent any
  stages {
    stage('build') {
      parallel {
        stage('build') {
          steps {
            sh 'pwd'
          }
        }

        stage('print') {
          steps {
            echo 'hello'
          }
        }

      }
    }

    stage('error') {
      steps {
        sh '''ls
echo "hello"'''
      }
    }

    stage('deploy') {
      steps {
        sh 'echo "deploying"'
        sleep 3
      }
    }

  }
}