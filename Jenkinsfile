pipeline{
    agent any
    stages{
        stage("Source code checkout"){
            steps{
                sh 'mkdir gmail_repo'
                sh 'cd gmail_repo'
                checkout([$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'github_synq', url: 'https://github.com/HarrYx384/yesbank.git']]])
            }
        }
        
        stage("push this code to sneo repo"){
            steps{
                sh 'pwd'
            }
           

        }
        
    }
}
