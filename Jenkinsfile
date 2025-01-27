pipeline {
    agent any

    stages {
        stage ('Checkout') {
            steps {
                checkout scmGit(branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/smore566/jenkinstest.git']])
            }
        }
    }
}