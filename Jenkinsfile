pipeline{
    agent any
    
    stages{
        stage("Build"){
            environment {
                mavenHome = tool "maven_home"
            } 
            steps{
                echo "${mavenHome}"
                sh '${mavenHome}/bin/mvn clean package'
                sh "docker build . -t tomcatwebapp:${env.BUILD_ID}"
                
            }

        }
    }
}