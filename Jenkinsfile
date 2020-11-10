pipeline {
   agent any
  
   stages {
       stage('List') {
           steps {
               sh 'ls -la /lab74/'
           }
       }
   }
   post {
       always {
           archiveArtifacts artifacts: 'generatedFile.txt',   onlyIfSuccessful: true
       }
   }

}


