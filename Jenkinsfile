pipeline {
    agent any

    stages {
        stage('Checkout code') {
            steps {
<<<<<<< HEAD
                checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/Venki22/PipelineDemo.git]])
           }
       }
=======
                checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/Venki22/PipelineDemo.git']])
           }
       }

    stage('Install Maven Build Tool') {
            steps { 
                sh 'wget https://dlcdn.apache.org/maven/maven-3/3.9.5/binaries/apache-maven-3.9.5-bin.tar.gz'
                sh 'tar -xzvf /root/.jenkins/workspace/testpipleline/apache-maven-3.9.5-bin.tar.gz'
             } 
           }
>>>>>>> ee18fb03d7911e6ab62b8048399b9e0254780056
    }
}    
