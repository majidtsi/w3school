pipeline {
  agent any
  stages {
    stage('build') {
      parallel {
        stage('build') {
          steps {
            echo 'primo step'
            echo 'primo step 2'
          }
        }

        stage('build 2') {
          steps {
            echo 'step build 2'
          }
        }

      }
    }

    stage('test1') {
      parallel {
        stage('test1') {
          steps {
            echo 'test1'
          }
        }

        stage('') {
          steps {
            echo 'test 2'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'debloy'
      }
    }

  }
}