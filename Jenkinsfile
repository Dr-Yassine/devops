pipeline{
    agent any
    stages{
        stage("clone"){
            steps{
                sh 'git clone  https://github.com/Dr-Yassine/devops.git'
                echo 'cloning done'
            }
        }
        stage("build"){
            steps{
                sh 'cd testapp && npm install'
                echo 'building done'
            }
        }
        stage("deploy"){
            steps{
                sh 'cd testapp  && npm start'
                echo 'deployment done'
            }
        }
    }
}