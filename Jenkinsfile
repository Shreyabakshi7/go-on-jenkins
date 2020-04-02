pipeline{
    agent any
    environment{
        GO11MODULES = 'on'
    }
    tools{
        go 'go-1.12'
    }
    stages{
        stage{
            steps{
                sh 'go build'
            }
        }
    }
}