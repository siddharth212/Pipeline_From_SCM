pipeline {
    agent any

    stages {
       
         
        stage('Hello') {
            steps {
                catchError{
                ech 'errors'
                }
                
            }
        }
        
        stage('Build') {
            steps {
                echo 'Building'
            }
        }
        
        stage('Deploying') {
            steps {
                echo 'Deploying the code'
            }
        }
        
        stage('Testing') {
            steps {
                echo 'Testing the code'
            }
        }
        
        stage('Release') {
            steps {
                echo 'Releasing the Code'
            }
        }
            
            
        
            
           
    }
}
