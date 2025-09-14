pipeline {
    agent none
    parameters{
      booleanParam(name: 'DEBUG_BUILD', defaultValue: true, description: '')
      choice(name: 'CHOICES', choices: ['one','two', 'three'], description: '')
    }

    stages {
        stage('STAGE_01') {
          agent { label 'slave1' }
            steps {
                sh '''
                    ls -lrt
                    echo $DEBUG_BUILD
                    sleep 2
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
