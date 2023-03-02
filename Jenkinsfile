ipeline {

   agent any

   stages {
          stage('SSH into remote host') {
            steps {
               script {
                 withCredentials([sshUserPrivateKey(credentialsId: 'node-js-pipeline', keyFileVariable: 'SSH_KEY')]) {
                     sh '''
                         ssh -o StrictHostKeyChecking=no -i $SSH_KEY ubuntu@13.233.126.171 "cd /home"
                         '''
   }
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

