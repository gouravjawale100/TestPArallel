pipeline {
    agent none
    stages {
             stage('Build and run') {
                    steps {
                        echo 'Inside Build and run stage'
                        script {
                            parallel(
                                Build: {
                                    echo 'Building windows project'
                                },
                                Deploy: {
                                    echo 'Deploying the build'
                                },
                                Test: {
                                    echo 'Testing the project'
                                }
                            )
                        }
                    }
                }
                stage('Build and run for second') {
                    steps {
                        echo 'Inside Build and run for second stage'
                        script {
                            parallel(
                                Build: {
                                    echo 'Building ubuntu project'
                                },
                                Deploy: {
                                    echo 'Deploying the build on ubuntu'
                                },
                                Test: {
                                    echo 'Testing the project on ubuntu'
                                }
                            )
                        }
                    }
                }
            }
        }
