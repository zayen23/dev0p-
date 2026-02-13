pipeline {
    agent any

    tools {
        maven 'M2_HOME'
        git 'DefaultGit'
    }

    stages {

        stage('Checkout') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/zayen23/dev0p-.git'
            }
        }

        stage('Build') {
            steps {
                sh 'mvn clean install'
            }
        }

    }
}

