pipeline {
    agent any

    script {
        properties([
            [
                $class: 'DatadogJobProperty',
                tagFile: 'tags.txt'
            ],
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
