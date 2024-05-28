pipeline {
  agent any
  stages {
    stage('Plan') {
      steps {
        echo 'I want to plan my app developement'
      }
    }

    stage('Code') {
      steps {
        echo 'developement team start coding'
      }
    }

    stage('Build') {
      steps {
        echo 'built the app'
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'testers test the app'
          }
        }

        stage('Deploy ') {
          steps {
            echo 'Deploy the war file'
          }
        }

        stage('Release') {
          steps {
            echo 'Release the code to web servers or app servers'
          }
        }

        stage('Operate') {
          steps {
            echo 'test app functionality'
          }
        }

      }
    }

  }
}