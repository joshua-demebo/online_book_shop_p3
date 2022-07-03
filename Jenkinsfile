pipeline {
  agent any
  tools {
    maven 'my_maven'
  }
  stages {
    stage('Compile') {
        steps {
        sh 'mvn compile'
        }
    }
    stage('Test') {
        steps { 
        sh 'mvn test'    
        }
    }
  post {
        always {
            junit 'build/reports/**/*.xml'
        }
  }

}

