pipeline {
    agent any

    stages {
       
         
        stage('Hello') {
            steps {
                
                script{
                    try{
                    ech 'hello'
                    }
                    
                    catch(err){
                        def data = err.getMessage()
                        writeFile(file: 'error.txt', text:data) 
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
