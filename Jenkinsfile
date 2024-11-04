pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Build completed '
      }
    }

    stage('test stages') {
      parallel {
        stage('test 2') {
          steps {
            echo 'runing test2'
          }
        }

        stage('test 1') {
          steps {
            echo 'runnig test1'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'deployment completed '
      }
    }

  }
}