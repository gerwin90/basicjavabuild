pipeline {
    agent any
    stages {
            stage('Stage 1') {
                steps {
                    echo 'Running on Jenkins Docker with Github Repo using VS Code Jenkins Runner'
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