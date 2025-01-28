pipeline {
    agent {
        label 'run-on-jenkins-master-do-not-use-without-very-good-reason'
    }
    stages {
        stage ('Goodbye') {
            steps {
                echo 'Goodbye World'
            }
        }
        stage ('Build') {
            steps {
                echo 'Building'
            }
        }
        stage ('Deploy') {
            steps {
                echo 'Deploying'
            }
        }
        stage ('Test') {
            steps {
                echo 'Testing'
            }
        }
        stage ('Release') {
            steps {
                echo 'Releasing'
            }
        }
    }
}
