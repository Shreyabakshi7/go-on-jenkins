pipeline {
    agent any
    stages {
        stage ('Git Checkout') {
            checkout([$class: 'GitSCM', 
            branches: [[name: '*/master']], 
            doGenerateSubmoduleConfigurations: false, 
            extensions: [], 
            submoduleCfg: [], 
            userRemoteConfigs: [[credentialsId: '64114f85-194b-4f95-ae38-dde677503d69', 
            url: 'https://github.com/Shreyabakshi7/go-on-jenkins.git']]])
            
        }
        stage ('Static Code Analysis'){
            echo 'Static Code analysis'
        }
        stage ('Build') {
            echo 'Build the code'
        }
        stage ('Unit Testing'){
            echo 'Unit Testing'
        }
        stage ('Deploy') {
            echo 'deploy code'
        }
    }
}