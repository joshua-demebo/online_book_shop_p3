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
                /* `make check` returns non-zero on test failures,
                * using `true` to allow the Pipeline to continue nonetheless
                */
           sh 'make check || true' 
           //junit '**Test/*.xml' 
       }
     }
   } 
}
