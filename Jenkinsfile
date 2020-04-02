pipeline {
    agent any
    environment {
        GO11MODULES = 'on'
    }
    tools {
        go 'go-1.14'
    }
    stages {
        stage('Build Stage') {
            steps {
                sh 'go build'
            }
        }
    }
}