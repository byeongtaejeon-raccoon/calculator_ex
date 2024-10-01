pipeline {
    agent any
    stages {
        stage('Setup') {
           steps {
               withPythonEnv('/usr/bin') {
                   sh 'echo "Job is starting" '
               }            
           }
        }
        stage("Unit test") {
            steps {
                withPythonEnv('/usr/bin') {
                    sh "python3 test_calculator.py"
                }
            }
        }
    }
}
