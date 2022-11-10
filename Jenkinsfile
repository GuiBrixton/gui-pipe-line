@Library('shared-lib@master') _
pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building... testes'
                script{
                    cowsay = load 'lib/cowsay.groovy'
                    text = cowsay.template("mu")
                    echo text
                }
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying.....'
            }
        }
    }
}
