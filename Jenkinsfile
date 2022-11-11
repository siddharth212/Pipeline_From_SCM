pipeline {
    agent any

    stages {
       
         
        stage('Hello') {
            steps {
                script{
                    try{
                        echo 'Hello World'
                        a
                    }
                    catch (err) {
            echo err.getMessage()
            echo "Error detected"
             def date = new Date()
                   def data = err.getMessage() + date
                   writeFile(file: 'error.txt', text: data)
                   echo 'done'
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
