pipeline {
    agent any

    stages {
        stage('gitcheckout'){
            steps{
                git branch: 'main', url: 'https://github.com/Rupeshsolanki/cerebrone-terraform-aws-lambda.git'
            }
        }
                
        stage('terraform init') {
            steps {
                sh "terraform init"
    
            }
        }
        stage('terraform apply'){
            steps{
                sh "terraform apply -auto-approve"
            
            }
        }
    }
}
