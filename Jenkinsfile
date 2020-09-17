pipeline {
    agent any
    stages {
            stage('WS Clean-Up') {
                steps {
                    bat 'git clean -fdx'
                }
            }
    }    
    options {
        buildDiscarder(logRotator(numToKeepStr: '3'))
        }
    post { 
        always { 
            cleanWs()
        }
    }
}