pipeline {
    agent any

    script {
        properties([
            [
                $class: 'DatadogJobProperty',
                tagProperties: "groovy=tag"
            ]
        ])
    }

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
            }
        }
    }
}
