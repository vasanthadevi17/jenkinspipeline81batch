pipeline {
  agent any
  stages {
    stage('plan') {
      steps {
        echo 'plan for pipeline'
      }
    }

    stage('code') {
      steps {
        echo 'preapre code for pipeline'
      }
    }

    stage('bulid') {
      steps {
        echo 'bulid code  for pipeline'
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'Test code for pipeline'
          }
        }

        stage('release') {
          steps {
            echo 'Release code for pipeline'
          }
        }

        stage('deploy') {
          steps {
            echo 'Deploy code for pipeline'
          }
        }

        stage('operate') {
          steps {
            echo 'operate cod for pipeline'
          }
        }

      }
    }

  }
}