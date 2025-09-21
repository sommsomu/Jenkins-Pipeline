pipeline {
        agent any

        stages {
            stage ('checkIn') {
                steps {
                    git branch: 'main', 
                    credentialsId: 'github_apps', 
                    url: 'https://github.com/sommsomu/JulyRepo.git'
                }
            }

            
            stage ('Parallel Execution') {
                parallel {
                    stage('Check code quality'){
                        steps {
                            sh '''
                            ls -lrt
                            pwd
                            sleep 5
                            '''
                        }
                    }

                    stage ('Build') {
                        steps{
                            sh '''
                            pwd
                            ls -lrt
                            sleep 6
                            '''
            
                        }
                    }
                    
                }
        
            }
 
        }
}
