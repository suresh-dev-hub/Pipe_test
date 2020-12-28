pipeline {
  agent any
  stages {
    stage('Stage1') {
      parallel {
        stage('Stage1') {
          steps {
            sh 'date'
            echo 'Print date'
            pwd()
          }
        }

        stage('Stage1.1') {
          steps {
            echo 'Paralel stage'
          }
        }

      }
    }

    stage('Stage2') {
      steps {
        sleep 5
      }
    }

    stage('Final') {
      steps {
        echo 'THis is final '
      }
    }

  }
}