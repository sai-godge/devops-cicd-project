pipeline {
    agent any

    stages {

        stage('Clone Repository') {
            steps {
                git branch: 'main', url: 'https://github.com/sai-godge/devops-cicd-project.git'
            }
        }

        stage('Build Container Image') {
            steps {
                sh 'podman build -t devops-webapp .'
            }
        }

        stage('Run Container') {
            steps {
                sh 'podman run -d -p 8081:80 devops-webapp || true'
            }
        }

    }
}
