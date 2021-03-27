pipeline {
    agent any
    stages {
        stage('git repo & clean') {
            steps {
              // sh "rm  -rf TicketBookingServiceJunitTesting"
                dash "git clone https://github.com/Shahrex/TestingProject.git"
                dash "mvn clean -f TestingProject"
            }
        }
        stage('install') {
            steps {
                dash "mvn install -f TestingProject"
            }
        }
        stage('test') {
            steps {
                dash "mvn test -f TestingProject"
            }
        }
        stage('package') {
            steps {
               dash "mvn package -f TestingProject"
            }
        }
    }
}
