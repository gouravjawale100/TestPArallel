pipeline {
    agent none
    stages {
      parallel(
      {
        stage('Build and run') {
            steps {
                parallel(
                    Build: {
                        echo 'Building windows project'
                    },
                    Deploy: {
                        echo 'deploying the build'
                    },
                    Test: {
                        echo 'Testing the project'
                    }
                )
            }
        }
        },
{
        stage('Build and run for second') {
            steps {
                parallel(
                    Build: {
                        echo 'Building ubuntu project'
                    },
                    Deploy: {
                        echo 'deploying the build on ubuntu'
                    },
                    Test: {
                        echo 'Testing the project on ubuntu'
                    }
                )
            }
        }
      }




        )
    }
}