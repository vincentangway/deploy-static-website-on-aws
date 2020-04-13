pipeline {
    agent any
    stages {
        stage('Linting HTML') {
            steps {
                sh 'echo "Running Linting HTML..."'
                tidy -q -e *.html
            }
        }
    }
}
