pipeline {
  agent any

  stages {
    stage('STAGE_1'){
      steps {
        sh '''
        ls -lrt
        pwd
        '''
      }
    }
  }
  stages {
    stage('STAGE_2'){
      steps {
        sh '''
        sleep 5
        '''
      }
    }
  }
}