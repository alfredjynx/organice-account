pipeline {
    agent any
    stages {
        stage('Build Discovery') {
            steps {
                build job: 'organice-discovery', wait: true
            }
        }
        stage('Jenkins Account') {
            steps {
                echo 'Jenkins Account'
            }
        }
        stage('Build') { 
            steps {
                sh 'mvn clean install'
            }
        }      
    }
}