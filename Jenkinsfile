pipeline {
    agent any

    stages {
        stage('Getting Repo Files') {
            steps {
                git branch: 'main', url: 'https://github.com/amraabdallah/node-jenkins-tutorial'
            }
        }
        
        stage('Building Code') {
            steps {
                sh "docker build -t mynodeapp:v1.0 ."
            }
        }
    }
}
