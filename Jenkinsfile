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
                
                
                    withMaven(globalMavenSettingsConfig: '--- Use system default settings or file path ---', jdk: '--- Use system default JDK ---', maven: 'Maven-3.8.7', mavenSettingsConfig: '--- Use system default settings or file path ---') {
 
                      sh 'mvn clean package'
                    }
            }
                
            
        }

    }
}
