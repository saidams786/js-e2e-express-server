
pipeline{
    agent{label 'nodejs_11'}
    
    stages {
        stage('scm'){
            steps{
                git branch: 'main' , url: 'https://github.com/saidams786/js-e2e-express-server.git'
           }
          }
         stage ('build'){
            steps{
                sh '''npm install
                      npm run build
                      npm pack'''
                }
            }
        }

}

