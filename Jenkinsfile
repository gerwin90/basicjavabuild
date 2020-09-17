pipeline {
    agent any
    stages {
            stage('Stage 1') {
                steps {
                    echo 'Running on Jenkins Docker with Github Repo'
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