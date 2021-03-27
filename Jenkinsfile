pipeline {
    agent any
    stages {
        stage('git repo & clean') {
            steps {
              sh "rm  -rf TicketBookingServiceJunitTesting"
            //    sh "git clone https://github.com/Shahrex/TestingProject.git"
           //     sh "mvn clean -f TestingProject"
            }
        }
        stage('install') {
            steps {
              //  sh "mvn install -f TestingProject"
            }
        }
        stage('test') {
            steps {
           //     sh "mvn test -f TestingProject"
            }
        }
        stage('package') {
            steps {
          //     sh "mvn package -f TestingProject"
            }
        }
    }
}
