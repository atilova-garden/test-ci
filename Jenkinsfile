pipeline {
     agent any
 
     stages {
         stage('Show Git Info') {
             steps {
                 script {
                     // Print commit hash
                     sh 'echo "Commit: $(git rev-parse HEAD)"'
 
                     // Print repo name from git remote
                     sh 'echo "Repo: $(basename -s .git `git config --get remote.origin.url`)"'
                 }
             }
         }

      stage('Test Echo') {
             steps {
                 script {
                     sh 'Test'
                 }
             }
         }
     }
 }
