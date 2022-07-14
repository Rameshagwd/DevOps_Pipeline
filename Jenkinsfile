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
        stage ('SonarQube Scan') {
            steps {
              sh 'mvn sonar:sonar -Dsonar.host.url=http://10.32.39.109:9000 -Dsonar.login=2604f36fcd297e623df6df4aa9269f9ad4de30c8'
              
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
        stage ('MVN Deploy') {
            steps {
                sh 'mvn deploy'
            }
        }
    }
    
}