pipeline {
    agent { label 'node-1' }
    stages {
        stage ('clone the code') {
            steps {
                git url: 'https://github.com/maramvenkatareddy/node_js.git',
                    branch: 'main'
            }
        }
        stage ('build the code') {
            steps {
                sh """
                pwd
                npm install
                npm start
                """
            }
        }
    }
}