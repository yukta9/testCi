pipeline {
    agent any
    stages {
        stage('Test Connection') {
            steps {
                echo ':white_tick: Jenkins Pipeline Triggered Successfully!'
                sh 'pwd'
                sh 'ls -la'
            }
        }
        stage('Dummy Build') {
            steps {
                echo ':rocket: Simulating build process...'
                sh 'echo "Building frontend..."'
                sh 'sleep 5'
                echo ':tada: Build complete!'
            }
        }
    }
    post {
        success {
            echo ':white_tick: Pipeline executed successfully!'
        }
        failure {
            echo ':x: Pipeline failed!'
        }
    }
}