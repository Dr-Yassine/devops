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
                sh 'cd devops/testapp && npm install'
                echo 'building done'
            }
        }
        stage("deploy"){
            steps{
                sh 'cd devops/testapp  && npm start'
                echo 'deployment done'
            }
        }
    }
}