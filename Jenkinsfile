pipeline{
    agent any 
    tools {
        maven 'maven'
        jdk 'java'
    }
    
    stages{
        stage("Build"){
            steps{
                sh 'mvn install'
            }
        }
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
}
           
