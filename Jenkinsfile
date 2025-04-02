pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'No build step needed for Python project'
            }
        }

        stage('Test') {
            steps {
                echo 'Setting up virtual environment and running pytest on Windows...'
                bat '''
                    python -m venv mlip
                    call mlip\\Scripts\\activate.bat
                    pip install --upgrade pip
                    pip install pytest numpy pandas scikit-learn
                    pytest
                '''
            }
        }

        stage('Deploy') {
            steps {
                echo 'No deploy step defined for this lab'
            }
        }
    }
}
