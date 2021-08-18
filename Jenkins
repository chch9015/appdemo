pipeline{
    agent any
    stages{
        stage('checkout the code'){
            steps{
                git branch: 'develop', URL: 'https://github.com/chch9015/appdemo.git'
            } 
        }
        stage('deploy to the appdemo server'){
            steps{
                sh 'scp /var/lib/jenkins/workspace/appdemo/insex.html root@10.1.3.224:/opt/'
            }
        }
    }
}