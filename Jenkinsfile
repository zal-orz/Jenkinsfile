pipeline {
    agent {
        docker { image 'node:20.10.0-alpine3.19' }
    }
    stages {
        stage('Test') {
            steps {
                script {
                    def nodeVersion = sh(script: 'node --version', returnStdout: true).trim()
                    echo "Node.js Version: ${nodeVersion}"
                }
            }
        }
    }
}
