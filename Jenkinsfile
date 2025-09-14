pipeline {
    agent none

    stages {
        stage('STAGE_01') {
          agent { label 'slave1' }
            steps {
                sh '''
                    ls -lrt
                    pwd
                    sleep 5
                '''
            }
        }

        stage('STAGE_02') {
          agent { label 'slave2' }
            steps {
                sh '''
                    pwd
                    sleep 5
                '''
            }
        }
    }
}
