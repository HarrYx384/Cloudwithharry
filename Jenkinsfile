pipeline{
    agent any
    stages{
        stage("Source code checkout"){
            steps{
                checkout([$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/HarrYx384/yesbank.git']]])
                
            }
        }
        
        
    }
}
