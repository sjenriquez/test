pipeline {
    agent any

    stages {
        properties([
          [
            $class: 'DatadogJobProperty',
            tagFile: 'tags.txt'
          ]
        ])
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
