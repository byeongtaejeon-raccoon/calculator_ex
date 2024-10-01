pipeline {
    agent any
    stages {
        stage("Unit test") {
            steps {
                withPythonEnv('/usr/bin/python3') {
                    sh "python3 test_calculator.py"
                }
            }
        }
    }
}
