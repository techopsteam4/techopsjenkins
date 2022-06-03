pipeline{
    agent any
    stages{
        stage('procesInfor'){
            steps{
                sh 'ps -ef'
            }
        }
    }
    stage('systemstatus'){
        steps{
            sh 'systemctl status jenkins'
        }
    }
 }
}
