pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                cd /var/jenkins_home/workspace/TestRun
                cat Hello.java
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