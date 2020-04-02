pipeline {
    agent any
    stages {
        stage ('Git Checkout') {
            steps{
                    checkout([$class: 'GitSCM', 
                    branches: [[name: '*/master']], 
                    doGenerateSubmoduleConfigurations: false, 
                    extensions: [], 
                    submoduleCfg: [], 
                    userRemoteConfigs: [[credentialsId: '64114f85-194b-4f95-ae38-dde677503d69', 
                    url: 'https://github.com/Shreyabakshi7/go-on-jenkins.git']]])
                }
            
        }
        stage ('Static Code Analysis'){
            steps{
                echo 'Static Code analysis'
            }
           
        }
        stage ('Build') {
            steps{
                echo 'Build the code'
            }
            
        }
        stage ('Unit Testing'){
            steps{
                echo 'Unit Testing'
            }
            
        }
        stage ('Deploy') {
            steps{
                echo 'deploy code'
            }
            
        }
    }
}