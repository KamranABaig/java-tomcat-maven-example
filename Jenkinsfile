pipeline {
    agent any
    stages {
        stage ('Build Servlet Project') {
            steps {
                bat 'mvn clean package'
  
            }
         
            post{
                success{
                    echo 'Now Archiving ....'

                    archiveArtifacts artifacts : '**/*.war'
                }
            }
        }
<<<<<<< HEAD:jenkinsfile
        
    
}
=======
    }
}
>>>>>>> 51c386cefeaf25b2fa40669e2c7ab05f0c1b8af4:Jenkinsfile
