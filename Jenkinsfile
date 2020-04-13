pipeline {
    agent any
    stages {
        stage('Upload to AWS.') {
            steps {
                sh 'echo "Hello world!"'
                sh '''
                    echo "Multiline shell steps works too"
                    ls -lah
                '''
                sh 'echo "Running AWS Upload to S3 Bucket..."'
            }
        }
    }
}
