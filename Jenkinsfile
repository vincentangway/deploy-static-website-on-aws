pipeline {
    agent any
    stages {
        stage('Upload to AWS.') {
            steps {
                sh 'echo "Running AWS Upload to S3 Bucket..."'
                withAWS(credentials:'myProfile') {
                    s3Upload(file:'index.html', bucket:'jenkinsbucket122', path:'path/to/target/index.html')
                }
            }
        }
    }
}
