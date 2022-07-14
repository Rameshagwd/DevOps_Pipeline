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
                sh 'mnv clean'
            }
        }
        stage ('MVN Compile') {
            steps {
                sh 'mnv compile'
            }
        }
        stage ('MVN Install') {
            steps {
                sh 'mnv install'
            }
        }
        stage ('MVN test') {
            steps {
                sh 'mnv test'
            }
        }
        stage ('MVN package') {
            steps {
                sh 'mnv package'
            }
        }
        stage ('MVN Validate') {
            steps {
                sh 'mnv validate'
            }
        }
    }
    
}