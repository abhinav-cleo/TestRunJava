pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                sh 'cd /var/jenkins_home/workspace/TestRun'
                sh 'javac Hello.java'
                sh 'java Hello'
                echo 'Printing Environment Details'
                echo "Running ${env}"
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
            }
        }
    }
}