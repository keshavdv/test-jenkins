pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
                sh 'echo "FILE DATA" > testfile'
            }
        }
    }
    
    post {
        success {
            input 'Continue?'
            echo 'Deploying....'
        }
    }
}
