pipeline {
    agent any

    stages {
        stage('Build Backend Image') {
            steps {
                sh 'docker build -t backend-image ./backend'
            }
        }

        stage('Run Backend Container') {
            steps {
                sh 'docker run --rm backend-image'
            }
        }
    }
}
