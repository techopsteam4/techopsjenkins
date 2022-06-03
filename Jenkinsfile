pipeline{
    agent any
    stages{
        stage('clone-Andine'){
            steps{
                checkout([$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'github-id', url: 'https://github.com/techopsteam4/techopsjenkins.git']]])
            }
        }
        stage('status'){
        steps{
            sh 'systemctl status jenkins'
            sh 'ps -ef'
        }
    }
    stage('akudo-processes'){
        steps{
            sh 'ps -ef'
            sh 'sudo systemctl status jenkins'
        }
    }
 }
}
