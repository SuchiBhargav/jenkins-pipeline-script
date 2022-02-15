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

    stage('') {
      steps {
        sh '''ls
echo "hello"'''
      }
    }

  }
}