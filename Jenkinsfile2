pipeline {
    agent none
    stages {
        stage('Build and run') {
            steps {
                script {
                    parallel(
                        '1 of 1': {
                            echo 'Building windows project'
                        },
                        '1 of 2': {
                            echo 'Deploying the build'
                        },
                        '1 of 3': {
                            echo 'Testing the project'
                        }
                    )
                }
            }
        }
        stage('Build and run part 2') {
            steps {
                script {
                    parallel(
                        '2 of 1': {
                            echo 'Building windows project'
                        },
                        '2 of 2': {
                            echo 'Deploying the build'
                        },
                        '2 of 3': {
                            echo 'Testing the project'
                        }
                    )
                }
            }
        }
    }
}
