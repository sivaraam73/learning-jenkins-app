pipeline {
    agent any

    stages {
        
        stage('Build') {
            
            agent{
                label 'docker-agent1' {
                image 'node:18-alpine'
                reuseNode true
                }
            }
        
        steps{
           sh '''
           ls -la
           node --version
           npm --version
           npm ci 
           npm run build
           ls -la
           '''


        }

            
        }
        
    }
}
