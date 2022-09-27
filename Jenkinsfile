pipeline {
    agent {
        label 'jenkins-agent.netology.askbow.io'
    }
    stages {
        stage('Git') {
            steps{
                git branch: 'main', credentialsId: '1812fb9e-68ae-4732-99dc-b7d0b0a8deb5', url: 'git@github.com:dborchev/09-ci-04-jenkins.git'
            }
        }
        stage('Molecule test'){
            steps{
                dir('roles/vector-role/') {
                sh 'molecule test -s default'
                }
                cleanWs()
            }
        }
    }
}