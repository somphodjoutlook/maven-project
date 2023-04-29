pipeline{
    agent any
    environment {
        PATH = "/var/jenkins_home/tools/hudson.tasks.Maven_MavenInstallation/Maven/bin:$PATH"
    }
    stages{
        stage("Build"){
            steps{
                cleanupWs()
                script {
                    sh 'mvn clean package'
                }
                
            }

        }
    }
}