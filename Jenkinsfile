pipeline {
    agent {
        docker {
            image 'node:6-alpine' 
            args '-p 3001:3001' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'sudo npm install --unsafe-perm=true --allow-root' 
            }
        }
    }
}
