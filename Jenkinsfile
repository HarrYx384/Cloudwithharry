pipeline{
    agent any
    stages{
        stage("Source code checkout"){
            steps{
                checkout([$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'github_synq', url: 'https://github.com/HarrYx384/yesbank.git']]])
                
            }
        }
        
        
    }
}
