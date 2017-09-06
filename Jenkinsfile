pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'building...'
      }
    }
    stage('unit test') {
      steps {
        parallel(
          "unit test": {
            echo 'unit testing...'
            
          },
          "functional test": {
            echo 'functional test'
            
          },
          "integrateion test": {
            sh '''echo "OK"
'''
            
          }
        )
      }
    }
    stage('deploy') {
      steps {
        sh '''echo "OK"
'''
      }
    }
  }
}