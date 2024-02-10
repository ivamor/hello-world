pipeline {
    agent any
    stages {
        /* "Build" and "Test" stages omitted */

        stage('Deploy - Staging') {
            steps {
                sh 'ls'
            }
        }

        stage('Sanity check') {
            steps {
                input "Do you really want to check current directory as well?"
            }
        }

        stage('Deploy - Production') {
            steps {
                sh 'pwd'
            }
        }
    }
}
