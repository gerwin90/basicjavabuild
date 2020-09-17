pipeline {
    agent any
    stages {
            stage('Stage 1') {
                steps {
                    echo 'Running on Jenkins Docker with Github Repo using VS Code Jenkins Runner'
                }
            }
            stage('Stage 2') {
                steps {
                    sh 'java -version'
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