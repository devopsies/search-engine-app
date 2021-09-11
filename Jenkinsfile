pipeline {
    agent any
    
    stages {
        stage ('Generate the test cases') {
            steps {
                sh( returnStdout: false, script: """#!/bin/sh
                    g++ generate.cpp -o generate
                    chmod u=x generate
                    ./generate
                    """.stripIndent()
                )
            }
        }
        stage ('Run the search engine') {
            steps {
                sh "g++ search.cpp -o search"
                sh "chmod u=x search"
                sh "./search"
            }
        }
        stage ('Verify the results') {
            steps {
                sh( returnStdout: false, script: """#!/bin/sh
                    if cmp -s RES.txt OUT.txt ; then echo SUCCESS ; else exit 1 ; fi
                    """.stripIndent()
                )
            }
        }
    }
}
