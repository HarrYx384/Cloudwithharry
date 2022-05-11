pipeline{
    agent any
    stages{
        stage("Source code checkout"){
            steps{
                sh 'mkdir gmail_repo'
                sh 'cd gmail_repo'
                checkout([$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'github_synq', url: 'https://github.com/HarrYx384/yesbank.git']]])
                sh 'rm -rvf .git'
                sh 'cp * /tmp/sneo'
            }
        }
        
        stage("push this code to sneo repo"){
            steps{
               sh "pwd"
                dir('/tmp/sneo') {
                   sh 'git init'
                   sh 'git remote add origin  https://github.com/vikash-sneo/Testing.git'
                   sh 'git checkout -b ${JOB_NAME}_${BUILD_ID}'
                   sh 'git add .'
                   sh ' git commit -m "added new files"'
                   sh 'git push origin ${JOB_NAME}_${BUILD_ID}'
            }
            }           

        }
        
    }
}
