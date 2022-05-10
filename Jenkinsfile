pipeline{
    agent any
    stages{
        stage("Source code checkout"){
            steps{
                checkout([$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[url: 'git@github.com:HarrYx384/yesbank.git']]])
                
            }
        }
        
        
    }
}
