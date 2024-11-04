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
        input(message: 'are you sure to deploy', ok: 'YES ,I\'am sure')
        echo 'deployment completed '
      }
    }

    stage('Notify for nrw build') {
      steps {
        echo 'build successs'
      }
    }

  }
}