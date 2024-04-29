pipeline {
    agent none

    stages {
        stage('Build and run') {
          parallel {
            stage('master-agent-pipeline') {
              stages{
                stage('Build') {
                steps {
                  echo 'Building windows project'
                  }
                }
                stage('Test') {
                  steps {
                    echo 'Testing windows project'
                 }
                }
	       }
              }
            stage('ubuntu-agent-pipeline') {
              stages{
                stage('Build') {
                steps {
                  echo 'Building ubuntu project'
                  }
                }
                stage('Test') {
                  steps {
                    echo 'Testing ubuntu project'
                 }
                }
               }
              }
             }
            }
           }
          }