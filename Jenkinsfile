pipeline {
    agent any 
    environment {
        S3_BUCKET = 'phsinghka.dev'
    }
    stages {
        stage('New Changes'){
            steps{
                sh 'echo "Lets Deploy it"'
            }
        }
        stage('Delete files in S3') {
            steps {
                script {
                    def awsCli = sh(script: 'which aws', returnStdout: true).trim()
                    sh "${awsCli} s3 rm s3://${S3_BUCKET} --recursive"
                }
            }
        }
        stage('Deploy To S3'){
            steps {
                script {
                    def awsCli = sh(script: 'which aws', returnStdout: true).trim()
                    sh "${awsCli} s3 sync . s3://${S3_BUCKET}"
                }
            }
        }
        stage('Invalidate Cloudfront Cache'){
            steps{
                sh'echo "cloudfornt code goes here. and here"'
            }
        }
    }
}