pipeline {
    agent none

    stages {
        stage('Build and run') {
          
                steps {

                 parallel(

                  Build: {
                    echo 'Building windows project'
                  }

                  sdfdsf: {
                    echo 'deploying the build'
                  }

                  Test: {
                    echo 'Testing the project'
                  }

                  )
                  
                  }
                }
                
                }
	       }
              
            