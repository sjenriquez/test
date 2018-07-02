pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                    script {
                        properties([
                            [
                                $class: 'DatadogJobProperty',
                                tagFile: "tags.txt"
                            ]
                        ])
                    }

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
