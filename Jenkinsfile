pipeline {
    agent any

    stages {
        stage ('Build and run generator') {
            steps {
                sh 'g++ generate.cpp -o generate'
                sh 'chmod u=x generate'
                sh './generate'
            }
        }
        stage ('Build and run search engine'){
            steps{
                sh 'g++ search.cpp -o search'
                sh 'chmod u=x search'
                sh './search'
            }
        }
        stage ('Running tests'){
            steps{
                sh 'if cmp -s RES.txt OUT.txt ; then echo SUCESS ; else exit 1 ; fi'
            }
        }
    }
}
