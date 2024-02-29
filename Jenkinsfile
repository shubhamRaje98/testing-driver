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
            script{
                def script = load "./test.groovy"
                groovyScript.execute()
            }
            
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}