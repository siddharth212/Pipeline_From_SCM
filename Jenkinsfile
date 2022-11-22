pipeline {
    agent any

    stages {
       
         
        stage('Hello') {
            steps {

                catchError(buildResult:'unstable',catchInterruptions:false, message:'stage failed', stageResult:'Failure'){
                ech 'errors'
                catchError{
                ech 'errorssss'  
               
                }
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
