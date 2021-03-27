pipeline {
    agent any
    stages {
        stage('git repo & clean') {
            steps {
              // bat "rm  -rf TicketBookingServiceJunitTesting"
                sh "git clone https://github.com/Shahrex/TestingProject.git"
                sh "mvn clean -f TestingProject"
            }
        }
        stage('install') {
            steps {
                bat "mvn install -f TestingProject"
            }
        }
        stage('test') {
            steps {
                bat "mvn test -f TestingProject"
            }
        }
        stage('package') {
            steps {
                bat "mvn package -f TestingProject"
            }
        }
    }
}
