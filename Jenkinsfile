pipeline {
    agent any
    stages {
        stage('git repo & clean') {
            steps {
              // sh "rm  -rf TicketBookingServiceJunitTesting"
                bat "git clone https://github.com/Shahrex/TestingProject.git"
                bat "mvn clean -f TestingProject"
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
