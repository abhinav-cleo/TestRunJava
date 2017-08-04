pipeline {
    agent any
    parameters {
            string(name: 'Greeting', defaultValue: 'Hello', description: 'How should I greet the world?')
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