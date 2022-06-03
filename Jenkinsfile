pipeline{
    agent any
    stages{
        stage('procesInfor'){
            steps{
                sh 'ps -ef'
            }
        }
        stage('status'){
        steps{
            sh 'systemctl status jenkins'
        }
    }
 }
}
