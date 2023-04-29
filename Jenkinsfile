pipeline{
    agent any
    
    stages{
        stage("Build"){
            environment {
                mavenHome = tool "maven_home"
            } 
            steps{
                sh "ls -a ${mavenHome}"
                sh '${mavenHome}/bin/mvn clean package'
                
            }

        }
    }
}