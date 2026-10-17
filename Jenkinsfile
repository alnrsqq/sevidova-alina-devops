pipeline {
    agent any
    
    environment {
        STUDENT_NAME = 'Alina'
        STUDENT_SURNAME = 'Sevidova'
        STUDENT_GROUP = 'IT2-2304' 
        STUDENT_ID = '37697'  
    }
    
    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }
        
        stage('Build') {
            steps {
                echo "Student: ${env.STUDENT_NAME} ${env.STUDENT_SURNAME}"
                echo "Group: ${env.STUDENT_GROUP}"
                echo "Student ID: ${env.STUDENT_ID}"
                echo 'Building project...'
            }
        }
        
        stage('Test') {
            steps {
                echo 'Running tests...'
            }
        }
        
        stage('Docker Build') {
            steps {
                echo 'Building Docker image...'
            }
        }
        
        stage('Docker Run') {
            steps {
                echo 'Running Docker container...'
            }
        }
    }
}
