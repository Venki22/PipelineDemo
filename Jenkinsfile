pipeline {
    agent any

    stages {
        stage('Checkout code') {
            steps {
                checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/Venki22/PipelineDemo.git']])
           }
       }
        stage('Install Maven Build Tool') {
            steps { 
                sh 'wget https://dlcdn.apache.org/maven/maven-3/3.9.5/binaries/apache-maven-3.9.5-bin.tar.gz'
                sh 'tar -xzvf /root/.jenkins/workspace/test/apache-maven-3.9.5-bin.tar.gz'
            } 
        }
        stage('Compile Sample Application') {
            steps {
                dir('/root/.jenkins/workspace/test/addressbook'){
                sh '/root/.jenkins/workspace/test/apache-maven-3.9.5/bin/mvn compile'
            }
        }
        
    }
  }
}   

