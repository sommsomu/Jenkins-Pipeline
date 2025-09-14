pipeline {
  agent any

  stages {
    stage('STAGE_01'){
      steps {
        sh '''
        ls -lrt
        pwd
        '''
      }
    }
  }
  stages {
    stage('STAGE_02'){
      steps {
        sh '''
        sleep 5
        '''
      }
    }
  }
}