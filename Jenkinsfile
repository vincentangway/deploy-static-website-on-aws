pipeline {
    agent any
    stages {
        stage('Linting HTML') {
            steps {
                sh 'echo "Running Tidy HTML..."'
            }
        }
        stage('Upload to AWS.') {
            steps {
                sh 'echo "Running AWS Upload to S3 Bucket..."'
                withAWS(region:'us-east-2', credentials:'aws-static') {
                    s3Upload(file:'index.html', bucket:'jenkinsbucket122', path:'index.html')
                }
            }
        }
    }
}
