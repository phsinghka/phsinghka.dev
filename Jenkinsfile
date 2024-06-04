pipeline {
    agent any 
    stages {
        stage('New Changes'){
            steps{
                sh 'echo "Lets Deploy it"'
            }
        }
        stage('Deploy To S3'){
            steps{
                sh'echo "s3 code goes here."'
            }
        }
        stage('Invalidate Cloudfront Cache'){
            steps{
                sh'echo "cloudfornt code goes here."'
            }
        }
    }
}