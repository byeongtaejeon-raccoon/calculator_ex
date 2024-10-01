pipeline {
    agent {
        docker {
            image 'btjeon/jenkins-agent-python'
            args '-u root --privileged'
        }
    }
    stages {
        stage("Unit test") {
            steps {
                sh "python3 test_calculator.py"
            }
        }
    }
}
