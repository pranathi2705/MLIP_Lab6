pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                bat '''
                echo Build Step: Python does not need compilation.
                '''
            }
        }

        stage('Test') {
            steps {
                bat '''
                echo Running tests with pytest...
                pytest
                '''
            }
        }

        stage('Deploy') {
            steps {
                bat '''
                echo Deployment step - no deployment needed for this lab.
                '''
            }
        }
    }
}
