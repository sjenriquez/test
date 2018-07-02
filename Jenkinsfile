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
                        [
                            $class: 'DatadogJobProperty',
                            tagProperties: "groovy=tag"
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
