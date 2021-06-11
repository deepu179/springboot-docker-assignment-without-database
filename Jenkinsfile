pipeline {
    tools { 
        maven 'maven-3.8.1' 
    }
    agent {
        label 'master'
    }
    stages{
        stage('git stage'){
            steps{
                git branch: 'main', url: 'https://github.com/deepu179/springboot-docker-assignment-without-database.git'
            }
        }
        stage('buils maven project'){
            steps{
                sh 'mvn clean package'
            }
    }
    
}
}
