pipeline {
    agent any
    stages {
        stage ('Build') {
            steps {
                 echo 'Build'
                 buildApp()
            }
        }
        stage ('Test') {
            steps {
                 echo 'Test'
            }
        }
    }
}

def buildApp() {
    def appImage = docker.build("minsikl/jenkins-test:${BUILD_NUMBER}")
}
