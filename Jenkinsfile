pipeline{
    agent any
    stages{
        stage('Git clone'){
            steps{
                git branch: 'main', url: 'https://github.com/Renatoksh/HelloProject.git'
            }
        }
        
        stage('maven Test'){
            steps{
                sh 'mvn test'
            }
        
        stage('Create Dockerimage'){
            steps{
                echo "Deploy the war file to the server"
            }
        }
        
    }
}
