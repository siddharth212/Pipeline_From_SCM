pipeline {
    agent any

    stages {
        script{
            try {
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
            }
            
            catch{
            stage('write') {
           steps {
               script {
                   def date = new Date()
                   def data = "Hello World\nSecond line\n" + date
                   writeFile(file: 'error.txt', text: data)
                   echo 'done'
               }
           }
       }
            
            }
        
        
    }
}
