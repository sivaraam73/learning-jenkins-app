pipeline {
    agent any

    stages {
        
        stage('Build') {
            
            agent{
               docker{}
                dockerfile true
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
