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
                script{

                    sh 'mvn test'
                    
                }
            }
        }
        stage('Integration testing'){
            
            steps{
                
                script{
                    
                    sh 'mvn verify -DskipUnitTests'
                }
            }
        }

    }
}
