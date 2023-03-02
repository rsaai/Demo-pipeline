pipeline {

   agent any

   stages {
         stage('install nodejs') {
           steps { 
             sh 'apt install nodejs'
             sh 'node -v'
                 }
             }
         stage('Install Dependencies') {
        steps {
           sh 'npm install'
        }
     }

     stage('Test') {
        steps {
           sh 'echo "testing application..."'
        }
      }

         stage("Deploy application") {
         steps {
           sh 'echo "deploying application..."'
         }

     }

        }

   }
