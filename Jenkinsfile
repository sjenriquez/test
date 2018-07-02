pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                properties([
                  [
                    $class: 'DatadogJobProperty',
                    tagFile: 'tags.txt'
                  ]
                ])
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
