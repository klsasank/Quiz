pipeline {
    agent any
    
    stages {
        stage('Clone') {
            steps {
                git 'https://github.com/klsasank/Quiz.git'
            }
        }
        stage('Build') {
            steps {
                echo 'Building project…'
                sh './build.sh' // Example shell script for building the project
            }
        }
        stage('Test') {
            steps {
                echo 'Test project…'


                sh './test.sh' // Example shell script for testing
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploy project…'

                sh './deploy.sh' // Example shell script for deployment
            }
        }
    }
}
