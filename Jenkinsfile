pipeline {
    

    stages {
        stage('STAGE_01') {
          agent { label 'slave1' }
            steps {
                sh '''
                    ls -lrt
                    pwd
                '''
            }
        }

        stage('STAGE_02') {
          agent { label 'slave2' }
            steps {
                sh '''
                    sleep 5
                '''
            }
        }
    }
}
