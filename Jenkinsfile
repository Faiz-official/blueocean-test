pipeline {
  agent any
  stages {
    stage('Checkout') {
      steps {
        echo 'Cloning repository...'
        checkout scm
      }
    }

    stage('Build') {
      steps {
        echo 'Installing dependencies...'
        sh 'npm install'
      }
    }

    stage('Test') {
      steps {
        echo 'Running tests...'
        sh 'npm test'
      }
    }

    stage('Deploy') {
      steps {
        echo 'Simulating deployment...'
        sh 'echo "App deployed successfully!"'
      }
    }

  }
  post {
    always {
      echo 'Pipeline complete!'
    }

  }
}