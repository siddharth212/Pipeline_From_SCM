pipeline {
    agent any
    
    try{

    stages {
       
         
        stage('Hello') {
            steps {
                echo 'Hello World'
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
            
            
         
            stage('write') {
           steps {
               
           }
       }
            
            
        
        
    }
    }
    
    catch(err){
        echo err.getMessage()
        echo "Error detected, but we will continue."
        
        script {
                   def date = new Date()
                   def data = "Errors should come Here\nSecond line\n" + date
                   writeFile(file: 'error.txt', text: data)
                   echo 'done'
               }
    
    }
        
        
        
        
        
}
