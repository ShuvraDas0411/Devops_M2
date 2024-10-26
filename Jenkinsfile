pipeline {
    agent any
    stages {
        stage('Clone Repository') {
            steps {
                git branch: 'master', url: 'https://github.com/ShuvraDas0411/Devops_M2.git'
            }
        }
        stage('Build with Maven') {
            steps {
                sh 'mvn clean package'
            }
        }
        stage('Deploy to Tomcat') {
            steps {
                echo 'Deploying WAR file to Tomcat...'
                // Add your deployment steps here
            }
        }
    }
}

