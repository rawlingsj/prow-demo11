pipeline {
    agent any
    environment {
      ORG               = 'rawlingsj'
      APP_NAME          = 'prow-demo11'
      CHARTMUSEUM_CREDS = credentials('jenkins-x-chartmuseum')
    }
    stages {
      stage('log') {
        steps {
          sh "env | sort"
          echo "foo"
          echo env.BRANCH_NAME
        }
      }
    }
  }
