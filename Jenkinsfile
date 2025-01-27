pipeline {
    agent any

    parameters {
        string(name: 'branch', defaultValue: 'main', description: 'The branch you want ot check in')
    }
    stages {
        stage ('Checkout') {
            steps {
                script {
                    checkout scmGit(
                        branches: [[name: "**/${params.branch}"]], extensions: [
                                                    [$class: 'CloneOption'],
                                                    [$class: 'CleanBeforeCheckout']
                        ],
                        userRemoteConfigs: [
                            [
                                url: 'https://github.com/smore566/jenkinstest.git'
                            ]
                        ]
                    )
                }
            }
        }
    }
}