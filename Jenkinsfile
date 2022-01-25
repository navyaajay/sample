pipeline {
    agent any
    tools{
        maven "Maven"
    }
    stages {
        stage('git Checkout') {
            steps {
                git url:'https://github.com/anandreddy143/warproject.git'
            }
        }
        stage("build") {
            steps {
                bat "mvn clean install package"
            }
        }
    }
}