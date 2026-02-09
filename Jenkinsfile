pipeline {
  agent any
  stages {
    stage('Plan') {
      steps {
        echo 'to plan for the application Development'
      }
    }

    stage('Code') {
      steps {
        echo 'To develop the application'
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'To test application fixes'
          }
        }

        stage('Deploy') {
          steps {
            echo 'To deploy the application'
          }
        }

        stage('Release') {
          steps {
            echo 'To release for production'
          }
        }

        stage('Operate') {
          steps {
            echo 'We can access apllication'
          }
        }

      }
    }

  }
}