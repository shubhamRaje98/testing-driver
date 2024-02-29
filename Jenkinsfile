pipeline {
    agent any

    stages {
        stage('get jar') {
            steps {
                bat 'cd'
                bat 'dir'
            }
        }
        stage('Test') {
            steps {
                def script = load "./test.groovy"
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}