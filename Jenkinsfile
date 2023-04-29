pipeline{
    agent any
    
    stages{
        stage("Build"){
            environment {
                mavenHome = tool "MAVEN"
            } 
            steps{
                sh "ls -a ${mavenHome}"
                sh '${mavenHome}/mvn clean package'
                
            }

        }
    }
}