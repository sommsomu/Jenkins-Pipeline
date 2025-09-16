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

    }

}