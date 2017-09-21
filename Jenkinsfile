pipeline {
  agent any
  stages {
    stage('Inicializar') {
      steps {
        echo 'Hello World'
      }
    }
    stage('Data') {
      steps {
        parallel(
          "Data": {
            sh 'date'
            
          },
          "Sleep": {
            sleep 10
            sh 'vaidarerro'
            
          }
        )
      }
    }
    stage('Finalizar') {
      steps {
        echo 'Terminei'
      }
    }
  }
}