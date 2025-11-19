pipeline {
    agent any
    tools{
        maven 'MAVEN-HOME'
    }
    stages {
        stage('git repo & clean') {
            steps {
                bat "git clone provide your github link"
                bat "mvn clean -f mavenjava"
            }
        }
        stage('install') {
            steps {
                bat "mvn install -f mavenjava"
            }
        }
        stage('test') {
            steps {
                bat "mvn test -f mavenjava"
            }
        }
        stage('deploy') {
            steps {
                bat "mvn deploy -f mavenjava"
            }
        }
    }
}
