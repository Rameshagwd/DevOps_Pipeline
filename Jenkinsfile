pipeline {
    agent any
    stages {
        stage ('Git Clone') {
            steps {
                git branch: 'main', url: 'https://github.com/Rameshagwd/DevOps_Pipeline.git'
            }
        }
        stage ('MVN Clean') {
            steps {
                sh 'mvn clean'
            }
        }
        stage ('MVN Compile') {
            steps {
                sh 'mvn compile'
            }
        }
        stage ('MVN Install') {
            steps {
                sh 'mvn install'
            }
        }
        stage ('MVN test') {
            steps {
                sh 'mvn test'
            }
        }
        stage ('MVN package') {
            steps {
                sh 'mvn package'
            }
        }
        stage ('MVN Validate') {
            steps {
                sh 'mvn validate'
            }
        }
    }
    
}