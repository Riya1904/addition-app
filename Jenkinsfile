pipeline {
    agent any
    triggers {
        cron('*/2 * * * *')
    }
    stages {
        stage('Clone Repo') {
            steps {
                git 'https://github.com/yourusername/addition-app.git'
            }
        }
        stage('Build') {
            steps {
                sh 'chmod +x build.sh'
                sh './build.sh'
            }
        }
    }
}
