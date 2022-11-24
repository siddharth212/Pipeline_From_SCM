pipeline {
    agent any

    stages {
       
         
        stage('Hello') {
            steps {
                
                script{
                    try{
                        echo 'try'
                    echo 'hello'
                    }
                    
                    catch(err){
                        echo 'in catch'
                        def data = err.getMessage()
                        writeFile(file: 'error.txt', text:data) 
                    }
                
                
               
                }
                
                
            }
        }
        
        stage('Build') {
            steps {
                
                try{
                     echo 'try'
                echov 'Building'
                    cdd /df
                }
                
                
                
                 catch(err){
                        echo 'in catch'
                        def data = err.getMessage()
                        writeFile(file: 'error.txt', text:data) 
                    }
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
