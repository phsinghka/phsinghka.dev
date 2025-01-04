pipeline {
    agent any 
    environment {
        S3_BUCKET = 'phsinghka.dev'
        CLOUDFRONT_DISTRIBUTION_ID = "E25FBF8MG5KDU6"
    }
    stages {
        stage('New Changes'){
            steps{
                sh 'echo "Lets Deploy it"'
            }
        }
        stage('Deploy To S3'){
            steps {
                script {
                    def awsCli = sh(script: 'which aws', returnStdout: true).trim()
                    sh "${awsCli} s3 sync . s3://${S3_BUCKET} --delete"
                }
            }
        }
        stage('Invalidate CloudFront Cache') {
            steps {
                script {
                    def awsCli = sh(script: 'which aws', returnStdout: true).trim()
                    sh "${awsCli} cloudfront create-invalidation --distribution-id ${CLOUDFRONT_DISTRIBUTION_ID} --paths '/*'"
                }
            }
        }
    }
}