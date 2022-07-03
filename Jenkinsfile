pipeline {
  agent any
  tools {
    maven 'my_maven'
  }
  stages {
    stage('Compile') {
<<<<<<< HEAD
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

=======
      steps {
        sh 'mvn compile'
    }
  } 
     stage('Test') {
       steps {
                /* `make check` returns non-zero on test failures,
                * using `true` to allow the Pipeline to continue nonetheless
                */
           sh 'make check || true' 
           //junit '**Test/*.xml' 
       }
     }
   } 
>>>>>>> 9be14e9711ef5afa887bfbaf0289f6edf998baec
}
