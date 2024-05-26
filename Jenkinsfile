 pipeline {    
    agent any 
    
    tools {
        jdk 'jdk17'
        maven 'maven3'
    }

    stages {
       
        
        stage('Compile') {
            steps {
            sh  "mvn compile"
            }
        }
        
        stage('tests') {
            steps {
                sh "mvn test"
            }
        }
        
        stage('Package') {
            steps {
                sh "mvn package"
            }
        }
    }
}
