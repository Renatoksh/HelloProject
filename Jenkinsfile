pipeline{
    agent any
    stages{
        stage('Git clone'){
            steps{
                git branch: 'main', url: 'https://github.com/Renatoksh/HelloProject.git'
            }
        }
        
        stage('maven build'){
            steps{
                sh 'mvn package'
            }
        }
        stage('Create Dockerimage'){
            steps{
                sh 'docker build -t thetips4you/springboot:latest .'
            }
        }
        
    }
}
