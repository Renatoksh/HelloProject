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
        }
        stage('mvn staging'){
            steps{
                "#!/bin/bash"
                echo "##########Detecting the OS Version######"
                cat /etc/redhat-release
                echo "##########Kernel Version########"
                uname -a    
            }
        }
        stage('Create Dockerimage'){
            steps{
                echo "Deploy the war file to the server"
            }
        }
    }
}
