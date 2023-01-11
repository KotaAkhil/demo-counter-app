pipeline{
    
    agent any 
    
    stages {
        
        stage('Git Checkout'){
            
            steps{
                
                git branch: 'main', url: 'https://github.com/KotaAkhil/demo-counter-app.git'
            }
        }
        /*stage('UNIT TESTING'){
            
            steps{
                

                    sh 'mvn test'

            }
            
        }
        stage('Integration testing'){
            
            steps{
                
                
                    
                    sh 'mvn verify -DskipUnitTests'
            }
            
        }*/
        stage('Maven build'){
            
            steps{
                
                
                    
                    sh script: 'mvn clean package'
                
            }
        }

    }
}
