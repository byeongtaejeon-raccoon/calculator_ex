pipeline {
    agent any
    stages {
        stage('Setup') {
           steps {
               withPythonEnv('/usr/bin/python3') {
                   sh 'echo "Job is starting" '
               }            
           }
        }
        stage("Unit test") {
            steps {
                withPythonEnv('/usr/bin/python3') {
                    sh "python3 test_calculator.py"
                }
            }
        }
    }
}
