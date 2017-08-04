pipeline {
    agent any
    parameters {
            string(name: 'Greeting', defaultValue: 'Hello', description: 'How should I greet the world?')
        }
    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                echo 'Printing Environment Details'
                sh 'printenv'
            }
        }
        stage('Test') {
            steps {
            }
        }
        stage('Deploy') {
            steps {
            }
        }
    }
}