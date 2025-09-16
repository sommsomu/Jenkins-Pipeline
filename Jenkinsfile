pipeline {
    agent any

    stages {
        stage ('Checkout'){
            steps{
               git branch: 'main', 
               credentialsId: 'github_apps', 
               url: 'https://github.com/sommsomu/JulyRepo.git' 
            }
        }

        stage ('build'){
            steps{
               sh '''
               ls -lrt
               '''
            }
        }
        stage ('checkout git'){
            steps{
               checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'github_apps', url: 'https://github.com/sommsomu/Jenkins-Pipeline.git']])
            }
        }

        stage ('Check code quality'){

            steps{
                '''
                pwd
                ls -lrt
                '''
            }
        }


    }

}