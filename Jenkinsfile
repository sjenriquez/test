pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                    script {
                        properties([
                            [
                                $class: 'DatadogJobProperty',
                                tagProperties: "groovy=tag"
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
