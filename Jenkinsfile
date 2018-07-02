pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                script{
                    properties([
                        [
                            $class: 'DatadogJobProperty',
                            tagFile: 'tags.txt'
                        ]
                    ])
                }
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
