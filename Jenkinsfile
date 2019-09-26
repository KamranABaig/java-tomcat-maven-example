pipeline {
    agent any
    stages {
        stage ('Build Servlet Project') {
            steps {
                bat 'clean package'
  
            }
         
            post{
                success{
                    echo 'Now Archiving ....'

                    archiveArtifacts artifacts : '**/*.war'
                }
            }
        }
    }
            
}
