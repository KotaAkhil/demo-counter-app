pipeline{
    
    agent any 
    
    stages {
        
        stage('Git Checkout'){
            
            steps{
                
                git branch: 'main', url: 'https://github.com/KotaAkhil/demo-counter-app.git'
            }
        }
        stage('UNIT TESTING'){
            
            steps{
                
                sh 'mvn test'
            }
        }

    }
}
