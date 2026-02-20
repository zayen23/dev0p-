pipeline {
    agent any
    tools {
        maven 'M2_HOME'
    }
    stages {
        stage('GIT') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/zayen23/dev0p-.git'
                
                sh 'mvn clean'
            }
        }
       stage('MVN SONARQUBE') {
    steps {
        sh 'mvn sonar:sonar -Dsonar.token=squ_cc97ba90103265066048661e5bf9226556bc4345'
    }
}
    }
}
