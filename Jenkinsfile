pipeline {
    agent { label 'slave1' }

    stages {
        stage('STAGE_01') {
            steps {
                sh '''
                    ls -lrt
                    pwd
                '''
            }
        }

        stage('STAGE_02') {
            steps {
                sh '''
                    sleep 5
                '''
            }
        }
    }
}
