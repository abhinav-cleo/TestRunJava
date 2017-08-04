pipeline {
    agent any
    parameters {
            string(name: 'Greeting', defaultValue: 'Hello', description: 'How should I greet the world?')
        }
    environment {
            FROM_EMAIL = 'cic@cleo.com'
            ACTIVATION_URL    = 'https://cleointegration.xyz'
        }
    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                sh 'cd /var/jenkins_home/workspace/TestRun'
                sh 'javac Hello.java'
                sh 'java Hello'
                echo 'Printing Environment Details'
                echo "Running ${env.BUILD_ID}"
                echo "printing the Environment Variables"
                sh 'printenv'
                echo "Printing the custom parameters"
                echo "${params.Greeting} World!"
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