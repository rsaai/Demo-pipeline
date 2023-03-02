pipeline {

   agent any

   stages {
         stage('install nodejs') {
           steps {
             sh 'apt install nodejs'
             #sh 'apt install npm'
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

