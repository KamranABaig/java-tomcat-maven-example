pipeline {
    agent any
    stages {
        stage ('Build Servlet Project') {
            steps {
                bat 'maven clean package'
  
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
