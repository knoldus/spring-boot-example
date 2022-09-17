pipeline{
    agent any 
    tools {
        maven 'maven'
        jdk 'java'
    }
    
    stages{
        stage("Compile"){
            steps{
                sh 'mvn clean compile'
            }
        }
        stage("Test"){
            steps{
                sh 'mvn clean test'
            }
        }
        stage("Package"){
            steps{
                sh 'mvn clean package'
            }
        }
    }
        post {
            success {
                echo "The Pipeline Is Success :"
            }
        }
}

           
