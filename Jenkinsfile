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
<<<<<<< HEAD
                    echo $DEBUG_BUILD
                    sleep 2
=======
                    pwd
                    sleep 5
>>>>>>> d87fe54dbd7bd43a03445422892773f9bbc34f8d
                '''
            }
        }

        stage('STAGE_02') {
          agent { label 'master' }
            steps {
                sh '''
                    pwd
                    sleep 5
                '''
            }
        }
    }
}
