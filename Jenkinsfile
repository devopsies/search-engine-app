pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
           steps {
                sh( returnStdout: false, script: """#!/bin/sh
                    echo gg
                    """.stripIndent()
                )
                sh "echo gg"
                )
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
