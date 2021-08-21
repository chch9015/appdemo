pipeline{
    agent any
    stages{
        stage('checkout the code'){
            steps{
                git branch: 'develop', url: 'https://github.com/chch9015/appdemo.git'
            } 
        }
        stage('deploy to the appdemo server'){
            steps{
                sh 'scp /var/lib/jenkins/workspace/dev-appdeploy/index.html root@10.1.3.224:/opt/'
            }
        }
    }
}