pipeline {
    agent none
    stages {
             stage('Build and run') {
                            parallel(

                                stage('1 of 1')
                               {
                                    echo 'Building windows project'
                                }
                                stage('1 of 2') {
                                    echo 'Deploying the build'
                                }
                                 stage('1 of 3') {
                                    echo 'Testing the project'
                                }
                            )
                        }

                        stage('Build and run part 2') {
                            parallel(

                                stage('2 of 1')
                               {
                                    echo 'Building windows project'
                                }
                                stage('2 of 2') {
                                    echo 'Deploying the build'
                                }
                                 stage('2 of 3') {
                                    echo 'Testing the project'
                                }
                            )
                        }





                    }
                }
                