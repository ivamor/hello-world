pipeline {
    agent { docker { agent1 } }
    stages {
        /* "Build" and "Test" stages omitted */

        stage('Deploy - Staging') {
            steps {
                sh 'cd /home/jenkins'
                sh 'ls'
            }
        }

        stage('Sanity check') {
            steps {
                input "Do you really want to open file?"
            }
        }

        stage('Deploy - Production') {
            steps {
                sh 'cat some_file.txt'
            }
        }
    }
}
