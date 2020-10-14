pipeline {
  agent any
  stages {
    stage('Manda e-mail') {
      steps {
        emailext(subject: 'Attento a quello che fai', body: 'Sei sicuro di star facendo un buon lavoro?', attachLog: true, from: 'marco.leonardo.porro@accenture.comq', to: 'markobau.mlp@outlook.it')
        sleep 5
      }
    }

    stage('Di\' ciao') {
      steps {
        libraryResource 'sayHello'
      }
    }

  }
  environment {
    bau1 = '27'
  }
}