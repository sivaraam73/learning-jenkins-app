pipeline {
     agent { dockerfile true}     
    stages {
        
        stage('Build') {
            
        
        
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
