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
               sh 'mvn sonar:sonar -Dsonar.token=squ_471a32e7ff00e7b503a02364763ddd6fff206578'
            }
        }
    }
}
