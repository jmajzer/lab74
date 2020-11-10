pipeline {
   agent any
  
   stages {
       stage('List') {
           steps {
               sh 'ls -la .'
           }
       }
   }
   post {
       always {
           archiveArtifacts artifacts: 'generatedFile.txt',   onlyIfSuccessful: true
       }
   }

}


